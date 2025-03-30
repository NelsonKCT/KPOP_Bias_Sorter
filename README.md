# K-pop Bias Sorter

A web-based tool to help K-pop fans determine their bias ranking through a series of choices. This sorter includes members from:

- IVE
- aespa
- (G)I-DLE
- Red Velvet
- ITZY
## Demo
[nelsonkct.github.io/KPOP_Bias_Sorter/](https://nelsonkct.github.io/KPOP_Bias_Sorter/)
## How It Works

1. You'll be presented with two K-pop idols
2. Choose your favorite between the two (or select "it's a tie")
3. Continue making choices until all idols are sorted
4. Get your personalized bias ranking!

## Development

This site is built with Jekyll. To run it locally:

```bash
# Using Docker
docker run --rm -it -p 4000:4000 -v $(pwd):/srv/jekyll jekyll/jekyll:3.8 jekyll serve --host 0.0.0.0

# Visit http://localhost:4000/kpop-bias-sorter/ in your browser
```

## Credits

- Original LOONA bias sorter by @skullface
- Modified by @nelsonkct 