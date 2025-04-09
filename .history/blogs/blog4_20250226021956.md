<h2 style="color: #245ab3;">Inconsistent JSON outputs and Headache</h2>
Date-26/02/25
<br><br>
You instruct an LLM to “return data as JSON,” but instead of clean JSON, it wraps the response in Markdown code blocks (json) or adds conversational fluff. You’re not alone, LOL.
<br><br>
The reason is that training data heavily consists of JSON markdown (triple tick with json ```json) often seen in readme files, stackoverflow. In my recent <b>AI Judge</b> project i allow openai and openrouter's api key , but the way to handle their outputs are completely different.Even the system prompts are different that's coz they respond differently. <br>
<b>Conclusion</b>: Write prompts to exlusively output in JSON markdown ------> 100% guarantee that ouput is in JSON markdown <br>
But if you ask to ouput in raw JSON (no markdown) there are chances you'll get ouput in raw and markdown JSON which will break your workflow.TC
<br><br>
Sometimes I find it amusing how i have to instruct the model like a baby !! That's why i wrote this tweet: 

<blockquote class="twitter-tweet" ><p lang="en" dir="ltr">engineers 2000s : hardcode stuff<br>engineers now : Dear god, let it be a JSON</p>&mdash; Hritij Rana (@HritijRana) <a href="https://twitter.com/HritijRana/status/1890800937452859874?ref_src=twsrc%5Etfw">February 15, 2025</a></blockquote> 

The ways we use to instruct LLM to respond in a certain format is amusing. Makes me cry at times. Structured output syntaxes don't do shit ! I've tried OpenRouter's Structured output and still it gives back JSON markdown and raw JSON alternatively.Resorting to <b>Dhamki</b> in prompts would assure you a better reponse. But then you'll be unable to show the prompts to people, lol . It's like how you make a baby to stop crying , everyone would resort to a different technique which may sound funny to others. 
<br><br>
