# `go takeahike`

I spent some time recently learning Go.  The tools and tutorials are nice, and the marketing budget is impressive.  But the actual programming was not fun.

Go gives you a handful of wooden blocks and a couple cans of playdough.  If you're the kind of developer who tends to impale him/herself with anything sharper than a crayon, it's a good language for you.  If, however, you are accustomed to working with full professional toolkit, you will find yourself hamstrung by the lack of all sorts of toys and goodies you've gotten used to using to make your life easier.  

It's not that I object to small languages; small languages are great.  It's just that Go shows very little creativity in choosing carefully a small set of features that work together to produce a rich, flexible, and colorful set of programing options.  Instead, it takes us back to the good old days, where were couldn't rely on programming languages to make our work easier, and instead built software as huge constructs of monochromatic tounge depressors.

Go takes the somewhat odd, but now familiar, design decisions of C and replaces many of them with equally odd alternatives.  What's up with `:=` declarations all over the place and their complicated scoping rules?  It's a clunky and complicated band-aid over excissively focus on statements.  Go dilutes the semantic simplicity of C with garbage collection, so that the mapping from Go to assembly in your head is much less transparent.  (I find GC to be convenient at times, but I've rarely found memory management to be a major challenge in my architectures, so I don't see what the big deal is.)  It bakes a few things into the language that could probably have been left as libraries&mdash;goroutines and channels&mdeash;while omitting lots of creature comforts that allows you to write concise that says what it does without additional ceremony.  It eschews real generality and instead forces you to write code in a specific style that by modern standards feels quite clunky and outdated.

Go also forces a huge pile of aesthetics.  On account of this unwelcome imposition, I feel quite entitled to pass judgement on Go's aesthetic chocies: it gets almost all of them wrong.  It strongly encourages your code to be ugly, and if you acceidentally write a lovely statement or two, `gofmt` will quickly fix that for you.  Code formatting is for humans to communicate with other humans, and computers do a bad job at it, so designing a language for ease of mechanical formatting is an ill-founded goal.  Consistency is no excuse for ugliness.

I can't think what I'd use Go for.  It's not a rich interpreted language, so not suitable for scripting or interactive use.  It doesn't have the structural facilities for large architectures.  It doesn't provide mechanisms for extension or hosting DSLs.  The code kind of makes my eyes hurt.  It compiles fast, which is nice, but this is less valueable for the small- to mid-sized programs it seems structually designed for.  Yes, it's easy to learn&mdash;but as a serious programmer, I'm happy to invest the time to learn a modern, sophisticated language with a solid conceptual foundation that will not only help me to write elegant code, but teach me to do it.
