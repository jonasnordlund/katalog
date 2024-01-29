# What is this?

Katalog is cross-platform user interface to intuitively generate SQL queries with the help of SqlKata. This underlying framework was chosen thanks to its comprehensive database support and that its expressive, [fluent interface](https://en.wikipedia.org/wiki/Fluent_interface) with method chaining also lends well to intuitive, graphical interfaces much like assembling Lego bricks.

# Background

It quickly became apparent to me that there is a severe lack of free, modern, and particularly _stand-alone_ query designers that would support "plug and play" scenarios as a subset in existing applications, commercial or not. Although graphical SQL query designers are fairly common, they are almost always part of an existing and powerful IDE environment that might far surpass the needs, or even _wants_, in a scenario where all you want is to provide user assistance in building custom SQL queries for e.g. reports.

# Usage

By using Katalog, you'll give your users a simple and intuitive way of assembling SQL queries, step by step like Lego bricks.

Just like in that system, some bricks only match others, but users will not have to care about this and are only presented with the choices that match the preceding one. For example, the query root will only allow the **Query** brick which will let a user specify which table or view to query. In turn, the **Query** brick will allow a **Getter** brick that will retrieve some or all rows in the result of the query, but also a **Condition** brick which will allow a user to filter the result or an **Order** brick which will set a result order. Many of these bricks can then be chained in a sequence, even supporting joins and grouping. A tower of these bricks is called a _sequence_ and in a final step, a user can combine multiple sequences with intersects, union, and except operators.

# Why not AI?

This is so 2010! Why not just describe what you want in natural language and let a language model generate the SQL?

At this time and even with powerful language models like GPT-4, allowing an AI to generate SQL queries can be hit and miss and in many contexts, "hoping for the best" or "being right 90% of the time" just isn't good enough. Hallucinations and misunderstandings are still unsolved problems in modern language models, and they are black boxes where you can only iterate on your prompt as you try to wrangle the correct response out of the AI. I personally think that _at this point in time_, we unfortunately still need a tool where the user in more directly involved in the query design.

Besides, the token cost for this tool is always $0 and Mother Nature will thank you.
