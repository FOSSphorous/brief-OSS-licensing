# brief-OSS-licensing
A not at all extensive introduction to the world of open source licensing for the lazy

#### Preface
I am not a copyright lawyer, or a lawyer at all for that matter (though I do have plans for that to change). I am definitely not your lawyer. If you're looking for official legal advice then you should go contact one of those. They'll let you know how much responsibility they feel like taking for anything that may come as a result of following it. 

For me, personally, that will be none.

At all.

## What If There's No License?

Your code/work becomes read-only as far as everyone else is concerned. Under most nations' copyright laws it will be "all rights reserved" for the person who wrote it. You really aren't supposed to make copies or utilize it in any way, outside of "fair use" exceptions which always require a court getting involved if flagged by the originator and disputed by the user/distributor. After a while it will end up in the public domain as free to use shareware. If you want to utilize unlicensed software that isn't in the public domain then you'll have to go to the source and get explicit permission to do so (in writing or some other permanent format if you don't want to risk expensive legal trouble later on). Developers will be reluctant to use it since you haven't given them real permission to do so. 

Usually a lack of a license happens because people aren't aware of the importance of licensing their code. A lot of people who intentionally don't bother licensing their code are usually in a camp where they're thinking to themselves "Of course people can use my code, I wouldn't/can't take anyone to courts for it. Feel free to."

If that describes you then that's very nice, a lovely sentiment.

Now please put that sentiment in text. Preferably in a document that says "LICENSE" and is out in the open for everyone to see.

Or, better yet, choose one of the already existing and extensively reviewed open source licenses that best fit your use-case.

## Copyright/Proprietary

You need permission to apply the code to places elsewhere and are often charged a fee for doing so. Restricts modifications and redisribution. Microsoft, AT&T and IBM were pioneers in the field of proprietary software licensing. Before then most software was just shareware without a license.

When you come across proprietary software it'll often (though, not always) be distributed in binary format, precompiled, and make you aware of the license via EULA (end user license agreement) or similar document.

## Copyleft/"share and share-alike" (can be further divided into "strong copyleft" and "weak copyleft") 
<strong>Examples:</strong>
<ul>  
  <li><a href="https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)">GPLv3</a></li>
  <li><a href="https://tldrlegal.com/license/open-software-licence-3.0">Open Software License (3.0)</a></li>
  <li><a href="https://creativecommons.org/licenses/by-sa/2.0/legalcode">CC BY-SA </a>(a Creative Commons license)</li>
  <li><a href="https://tldrlegal.com/license/mozilla-public-license-2.0-(mpl-2)">Mozilla Public License (2.0)</a></li>
</ul>

Any derivatives must allow redistribution of the software as well as modifications, and the license will have to be retained (in most cases). Some of the stronger licenses like the GPL absorb copycenter (like the BSD) so make sure you're aware of the code you make use of. You can find them in anything GNU, and the linux kernel [uses the GPLv2](https://www.kernel.org/doc/html/v4.16/process/license-rules.html) as of this time.

The GPL more or less amounts to "sure, you can have this thing but if you do something with it then send me your changes back and have everyone be able to see the source code." Which is a good way of ensuring your work will stay open source.

## Copycenter/Permissive
<strong>Examples:</strong> 
<ul>
  <li><a href="https://tldrlegal.com/license/bsd-2-clause-license-(freebsd)>BSD 2-Clause</a></li>
  <li><a href="https://tldrlegal.com/license/apache-license-2.0-(apache-2.0)">Apache license (2.0)</a></li>
  <li><a href="https://tldrlegal.com/license/mit-license">MIT license</a></li>
  <li><a href="https://unlicense.org/">Unilicense</a></li>
</ul>

The software is free to use still. The license is often a bit more flexible than a copyleft, not requiring that the code be distributed/available. [This category has](https://resources.whitesourcesoftware.com/blog-whitesource/open-source-licenses-trends-and-predictions) [been the most used](https://resources.whitesourcesoftware.com/blog-whitesource/top-10-open-source-software-licenses-of-2016-and-key-trends) for years because it allows people to use open source software without affecting the distribution by requiring that they need to disclose it in source code format (e.g. one can just give out pre-compiled binaries). BSD licensed code for example is found used in Sony's products (e.g. [the playstation 4](https://doc.dl.playstation.net/doc/ps4-oss/index.html)), Nintendo's ([the Switch](https://wololo.net/wagic/wp-content/uploads/2017/03/nintendo_switch_freebsd_hack.jpg) and [DS](https://www.nintendo.com/consumer/downloads/manual-nintendo-2ds-operations-english.pdf)(page 77)), [Ap](https://developer.apple.com/library/archive/documentation/MacOSX/Conceptual/OSX_Technology_Overview/SystemTechnology/SystemTechnology.html#//apple_ref/doc/uid/TP40001067-CH207-BCICAIFJ)[p](https://developer.apple.com/library/archive/documentation/Darwin/Conceptual/KernelProgramming/BSD/BSD.html)[l](https://github.com/apple/darwin-xnu/search?q=bsd)[e](https://opensource.apple.com/source/Libc/Libc-320/string/FreeBSD/) and [Microsoft](https://lwn.net/Articles/245805/) have BSD licensed code bundled with their operating systems, Netflix mingles with FreeBSD since [they use it for their servers](https://invidious.snopyta.org/watch?v=vcyQBup-Gto), etc.. Often gets treated as "shareware" in some circles, but it is not to be equated with "public domain" content. While items in the public domain are similarly free to use for all, they have no owner(s)/ownership. **Permissive licenses *do* have an owner.** 

The BSD licenses nowadays boil down to "Don't claim you wrote this. Don't blame me if it breaks. Don't use my name to promote your product."

# How to choose a license / What licenses are available?
Think to yourself about what you want your software to accomplish. 

Do you want to ensure that everyone can be sure of what's within the code they're getting no matter what happens to it? 

Do you want to make sure that it can be used for things you might not have thought of it being used for? (For the sake of example, imagine building something with cars in mind and someone realizing that it would work in ships and airplanes too.)

Is this a hobby project and/or you just want your software to be available to whoever can make use of it, regardless of if they give back code or not? (a "private use" clause.)

Do you want people to even be able to make changes to your code?

Do you want to be noted as the person who created the software, or are you fine with not being explicitly acknowledged so long as they don't claim to have written it? Maybe you don't care about credit. 

If you're working with/for a community, what licenses are common/acceptable within them?

There's a lot that can go into the decision and a lot of licenses for you to choose from that fit your specific (or general) needs.
That said, I advise against coming up with your own unique licenses. Whenever a new license pops up people need to do costly work to evaluate how enforcable they are and what licenses they're compatible with. There are thousands of licenses out there. Not exactly cheap or fun times.

## Places to look at
This is an incomplete briefing, so I think it's best to link to other sources where you can maybe get something a bit more in depth. The following are some of my favourites to refer people to.
<ul>
  <lh>Sites</lh>
  <li><a href="https://tldrlegal.com/">TLDR Legal</a></li>
  <li><a href="https://choosealicense.com/">Choose-A-License</a></li>
  <li><a href="https://opensource.org/licenses">OpenSource.org</a></li>
  <li><a href="https://opensource.guide/legal/">Open Source Guide</a></li>
  <li><a href="https://snyk.io/learn/open-source-licenses/">Open Source Licenses: Types and Comparison</a> - a similar guide</li>
  <br/><lh>Youtube Videos (linked through <a href="https://github.com/iv-org/invidious">Invidious</a>, a "free" youtube frontend)</lh>
  <li><a href="https://invidious.snopyta.org/watch?v=cJIi-hIlCQM">CppCon 2015: Kevin P. Fleming “A Crash Course in Open Source Licensing"</a></li>
  <li><a href="https://invidious.snopyta.org/watch?v=OnmWFxlG2GA">How to Choose an Open Source License | HackBeanpot 2018</a></li>
  <li><a href="https://invidious.snopyta.org/watch?v=9kGrKBOytYM">Felix Crux What You Need to Know About Open Source Licenses PyCon 2016</a></li>
</ul>
