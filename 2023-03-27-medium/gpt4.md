The below is my conversation with ChatGPT model 4 (as of 2023-03-24) to the best of my Markdown-formatting abilities:
___
Me:
>You are an editor and copy-writer. I have an article for you to improve, so it comes across to the reader even better. The style is clear and consise, yet humourous and relatable. The purpose of the article is to highlight one of the benefits of open source contributions, as well as attract new employees to the mentioned companies. For formatting I use markdown-syntax. You may do the output using your normal layout with bold typefaces and paragraphs. There is 1 Illustration I have left out, leaving only the alt-text in []-brackets. I'll give you the current version of the article in 3 chunks, first line indicating the progress (e.g 1 of 3). Just respond "OK" when you are ready to recieve the next section. After the 3rd section, please apply your editing and copy-writing magic. OK?

GPT 4:
>OK

Me:
>1 of 3
>
>&#35; Employee branding — another way to think about open source in the enterprise
>
>When contributions are made under the name of the enterprise, as demonstrated in this article, both the enterprise and employee receive recognition and exposure.
>
>This is an additional way of benefitting from open source, beyond the “zero cost” access to software. The enterprise gets exposure to a large pool of talent familiar with, or even experts in, relevant technologies. The employees themselves become more visible and can demonstrate their personal skills, which in turn also should increase the enterprise’s ability to attract top talent (the theory being that demonstrating the enterprise-talent will engage more people aspiring to develop or continue their career at that presumably attractive level). Win-win-win!
>
>&#35;&#35; Backstory (condensed)  
>I am helping Telenor to have autonomous teams deliver features to market faster. One frequent bottleneck is legacy systems, and one such system, dating back 10–15–20 years, is almost entirely based on SAP ASE (formerly known as Sybase SQL server).
>
>My “architectural archeology”-endeavor needed a dependency graph based on the realities of code, not (possibly) outdated documentation. The tool I choose was ANTLR4, with its concept of grammars and language-specific modules supporting various file-formats, including the t-sql syntax shared by SAP ASE and the more well-documented MS SQL server.
>
>I hit a few cases where the ANTLR4-grammar did not support all the ASE t-sql dialect quirks we use. Having the source code and ability to do my own changes, it was relatively easy to identify and fix these issues.
>
>To avoid maintaining my own version, constantly retrofitting and integrating changes from the rest of the community, I wanted to contribute the changes back. As Telenor is on a path to become even more developer-oriented, I got full support for this approach. I guess, luckily, only people from the enterprise-world understand the significance of this…
>
>Anyway, through this slightly convoluted chain of events, I found the opportunity to demonstrate how an enterprise can get additional value from open source by engaging through their organizational account on GitHub!

GPT 4:
>OK

Me (in this and the following part, I accidentally pasted headings formatted with &#42;&#42;-annotation and not &#35;&#35;...):
>2 of 3
>
>&#42;&#42;A practical example on how to engage&#42;&#42;  
>For those familiar with GitHub, the original material is at https://github.com/antlr/grammars-v4/pull/3199.
>
>For the less GitHub-versed, below is a “pull request”. It is a request from me (as a contributor) to the maintainer(s) of the project (antlr/grammars-v4), asking them to accept my change and include it in the official project. I have highlighted the key “employee branding wins” for an enterprise:
>  
>&nbsp;  
>[Annotated screenshot of GitHub PR]
>
>1&#41; Win 1: I have requested to take the changes from the TelenorNorway repository, signaling that the change originates from the TelenorNorway organization.
>
>2&#41; Win 2: I got some feedback on my changes. Engaging with the community is a good way to learn and grow as a developer, and to be a good ambassador for your organization. This is open for the world to see though, and I must admit I am usually quite anxious after sending off a PR, including this one!
>
>3&#41; Win 3: I get credited as the individual contributor, adding to my track record.
>
>&#42;&#42;Things to be aware of&#42;&#42;  
>I came across two practical matters to watch out for: Git-identities and test data management.
>
>Usually, and as was the case in the example, the need to do the change in the first place arises from an actual use-case. In this instance, I found some legacy code I wanted the ANTLR4-framework to support. While the real code is the ultimate test, for obvious reasons I can not add it to the open-source codebase. At the same time, I need to provide tests so the changes I do are not accidentally broken by someone else in the future. Hence the need to be cautious to do proper abstraction and generalization, while still making sure the fix addresses the original issue. It is very easy to add internal code as a test-case and forget to remove it (no worries, I avoided this temptation)!

GPT 4:
>OK

Me:
>3 of 3
>
>Another, and perhaps less obvious case I came across, was that of committer identity. Internally we also use Git, although with our corporate identities. This may or may not be desirable when publishing externally (e.g. if requiring the use of real-name or email as the internal committer name). In the example above I used my personal GitHub identity. This might be left to the individual committer’s personal preference, wanting to preserve the public track record across employments or using a handle instead of a real identifiable name. Or there might be policies in place that must be considered, such as a (perhaps misguided) policy mandating using real-name corporate identities externally, for added “brand value”.
>
>I did struggle with the multi-identity setup. For reference, a comprehensive guide I think may help is at https://medium.com/expedia-group-tech/how-to-handle-multiple-git-accounts-385afe430d5a
>
>&#42;&#42;Conclusion&#42;&#42;  
>As shown, contributing to open-source projects is beneficial for all participants, and at many levels. These include: tangible improvements to the open-source project, fixing bugs and expanding features. For the contributor, demonstrating and growing their skillset when interacting with a wider community. And especially in this case: for the enterprise itself by attracting the attention of talent familiar with the various open-source building blocks they rely on.
>
>With a few precautions it is safe and straight forward to engage with the open-source community in a much more rewarding capacity than merely using the code as-is!
>
>&#42;&#42;Found this interesting?&#42;&#42;  
>If you are a technologist or open-source contributor and got excited about this, then both Telenor and Accenture have open positions that may be a good fit! For the most recent list of vacant positions, please see https://www.telenor.com/career/recruitment/vacant-positions/ for all Telenor positions, and https://www.accenture.com/no-en/careers/explore-careers/area-of-interest/technology-careers for positions in Accenture (linked directly to “Technology Careers”. The top-level landing page for all skills is https://www.accenture.com/no-en/careers). Use filters to find applicable roles for your location and interest. We both hire to multiple locations globally!
>
>Also (in Norwegian — and valid at the time of publishing), Telenor has a new dedicated landing-page for IT positions; https://www.telenor.no/om/jobbitelenor/ledig-stilling-it/ and an open position for Tech Lead that should be spot-on if this article resonated with you: https://www.telenor.com/career/recruitment/vacant-positions/job-search-article.page?id=J107864
>
>…and one final thing; I’m featured in a photo on the landing-page mentioned AND to truly bring it full circle, when the picture was taken I was actually coding the change mentioned in this very article! What a time to be alive!
>
>&#42;&#42;Disclaimer&#42;&#42;  
>At the time of publishing, I am a shareholder of both Accenture and Telenor.
>
>&#42;&#42;Change log&#42;&#42;  
>2023–03–20: Originally published

GPT 4:
># Boost Your Brand with Open Source: A Win-Win for Companies and Employees
>**Discover how open source contributions can elevate both your company and employee branding, while attracting top talent to your team.**
>
>When employees contribute to open source projects under their company's name, everybody wins. Both the organization and the individual gain exposure and recognition, attracting potential employees to the company while showcasing existing employees' skills. Sounds like a winning strategy, right?
>
>## From Legacy Systems to GitHub PRs: A Tale of Open Source Contributions
>To give you a little backstory, I was assisting Telenor in speeding up feature delivery by utilizing autonomous teams. A common bottleneck: outdated systems, like a 10–20-year-old SAP ASE (formerly Sybase SQL server). To create a dependency graph based on the code (not unreliable documentation), I employed ANTLR4, with its grammars and language-specific modules, like t-sql syntax for SAP ASE and MS SQL server.
>
>I encountered a few ANTLR4-grammar cases that didn't support all ASE t-sql dialect quirks we used. By fixing these issues with the source code, I decided to contribute the changes back to avoid maintaining my own version. With Telenor's full support, I demonstrated how a company can gain additional value from open source by engaging through their GitHub organizational account.
>
>### A Real-World Example: The GitHub Pull Request
>
>Check out the original material on GitHub: https://github.com/antlr/grammars-v4/pull/3199.
>
>For GitHub newbies, a pull request (PR) asks the project maintainers to accept your changes and incorporate them into the official project. The PR in question highlights key "employee branding wins" for a company:
>
>1) *Win 1*: The changes come from the TelenorNorway repository, signaling the company's involvement.
>
>2) *Win 2*: The community's feedback helps employees learn and grow while being ambassadors for their organization.
> 
>3) *Win 3*: Individual contributors are credited, enhancing their professional track record.
> 
>### Proceed with Caution: Git-Identities and Test Data Management
>
>When contributing, be mindful of Git-identities and test data management. For instance, avoid adding internal code to the open-source codebase and ensure proper abstraction and generalization. Additionally, consider whether to use corporate or personal Git identities when publishing externally.
>
>For help managing multiple Git identities, check out this guide: https://medium.com/expedia-group-tech/how-to-handle-multiple-git-accounts-385afe430d5a.
>
>### The Open Source Win-Win
>
>As demonstrated, open source contributions benefit everyone involved: the project itself, the contributor, and the company. And with a few precautions, engaging with the open-source community can be safe, straightforward, and rewarding.
>
>### Ready to Join the Open Source Movement?
>
>If you're a technologist or open-source contributor excited by this concept, both Telenor and Accenture have open positions that might be a perfect fit! Check out Telenor's vacancies at https://www.telenor.com/career/recruitment/vacant-positions/ and Accenture's technology careers at https://www.accenture.com/no-en/careers/explore-careers/area-of-interest/technology-careers.
>
>Browse positions and use filters to find roles that match your location and interests. Both companies hire globally!
>
>*Disclaimer: At the time of publishing, I am a shareholder of both Accenture and Telenor.*

Me:
>Thanks! Can you also please condense it down to the bare essentials, with minimal storytelling and personal touch?

GPT 4:
># Boost Your Brand with Open Source Contributions
>**Open source contributions can enhance company and employee branding while attracting top talent.**
>
>## The Benefits of Open Source Contributions
>1) Company gains exposure and recognition by contributing under their name.
>2) Employees showcase their skills and gain visibility.
>3) The company attracts potential employees familiar with relevant technologies.
>## Key Points for Successful Contributions
>1) Choose a project that aligns with the company's tech stack and goals.
>2) Create a pull request on GitHub to propose changes and demonstrate the company's involvement.
>3) Engage with the open-source community for valuable feedback and learning opportunities.
>4) Credit individual contributors to enhance their professional track record.
>## Precautions
>1) Be mindful of Git-identities when publishing externally (corporate vs. personal).
>2) Manage test data carefully to avoid adding internal code to open-source projects.
>## Conclusion
>Open source contributions benefit everyone involved, and with the right approach, companies can safely and effectively engage with the open-source community.
>
>### Interested in Open Source?
>
>Check out open positions at Telenor and Accenture for technologists and open-source contributors:
>
>* Telenor: https://www.telenor.com/career/recruitment/vacant-positions/
> 
>* Accenture: https://www.accenture.com/no-en/careers/explore-careers/area-of-interest/technology-careers
___
[Back Home](./../README.md)