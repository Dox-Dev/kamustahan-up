<script>
    import { Accordion, AccordionItem } from '@skeletonlabs/skeleton';
</script>

<Accordion autocollapse>
    <AccordionItem>
        <svelte:fragment slot="lead"><i class="fa-solid fa-file-word"></svelte:fragment>
        <svelte:fragment slot="summary">Can you give at least 3 words to describe the past month/week?</svelte:fragment>
        <svelte:fragment slot="content">
            <h2 class="h2">
                <span class="bg-gradient-to-br from-blue-500 to-cyan-300 bg-clip-text text-transparent box-decoration-clone">Confusion.</span>
            </h2>
            <h2 class="h2">
                <span class="bg-gradient-to-br from-red-500 to-yellow-500 bg-clip-text text-transparent box-decoration-clone">Rest.</span>
            </h2>
            <h2 class="h2">
                <span class="bg-gradient-to-br from-pink-500 to-violet-500 bg-clip-text text-transparent box-decoration-clone">Fun.</span>
            </h2>
        </svelte:fragment>
    </AccordionItem>
    <AccordionItem>
        <svelte:fragment slot="lead"><i class="fa-solid fa-brain"/></svelte:fragment>
        <svelte:fragment slot="summary">How have you been or what's on your mind lately?</svelte:fragment>
        <svelte:fragment slot="content">
            Honestly, I've been fine these past few days. 
            Maybe a bit too comfortable for my own good, but I've been trying to do whatever's in my academic to-do list at the moment. 
            I should also probably tend to my thesis/research study, since I do still need to do some work in that regard.
            All-in-all, I've been enjoying all the free time I've suddenly gotten from the 2-week break and been using it to slowly, but surely, catch up on acads, org work, and life.
        </svelte:fragment>
    </AccordionItem>
    <AccordionItem>
        <svelte:fragment slot="lead"><i class="fa-solid fa-person-praying"/></svelte:fragment>
        <svelte:fragment slot="summary">Who or what are you thankful for right now and why?</svelte:fragment>
        <svelte:fragment slot="content">
            I'm thankful for the rest that I've been giving by this almighty break, as well as my friends and family for helping me enjoy it.
            In particular, I went to Hans' birthday celebration, sleepover, thingamajig on his birthday and spent time with the bois (and the so-called child).
            Then, I've been having fun revisiting some old titles that I enjoy like Terraria with a mix of Lethal Company and PlateUp. 
            Lastly, right now actually, I'm typing this very kamustahan in my family's private resort during our staycation (shameless plug: <a href="https://www.facebook.com/profile.php?id=61555294425232">Sunrise Blue Family Resort</a>).
        </svelte:fragment>
    </AccordionItem>
    <AccordionItem>
        <svelte:fragment slot="lead"><i class="fa-solid fa-trophy"/></svelte:fragment>
        <svelte:fragment slot="summary">Could you share any recent personal achievements or experiences?</svelte:fragment>
        <svelte:fragment slot="content">
            For the most part though, I've been doing alright.
            I don't think I made much personal achievements recently per se, but I have been able to catch up on my sleep.
            I was also able to catch up with friends whom I haven't talked to in a while over a few drinks (thanks Hans for the party).
            There's something else that I'd wanna share but that's probably something that's best left for the next kamustahan.
            Just let me cook. 
            <span><i class="fa-solid fa-fire"/> <i class="fa-solid fa-fire"/> <i class="fa-solid fa-fire"/></span>
        </svelte:fragment>
    </AccordionItem>
    <AccordionItem>
        <svelte:fragment slot="lead"><i class="fa-solid fa-briefcase"/></svelte:fragment>
        <svelte:fragment slot="summary">How are you managing your workload acads-wise or org-wise?</svelte:fragment>
        <svelte:fragment slot="content">
            Academics-wise, I honestly need to catch up. 
                I still need to worry about my part of the thesis, which I'm kind of guilty of not doing for the past few weeks. 
                So that's mostly what I've been doing starting today.
                Also, I need to do my lightning presentation for CS 132, as well as contribute a bit to my group's output.
            Org-wise, I've also got a bit of catching up to (although for DevelUP, I'm pretty on-track).
                For <b>UP CURSOR</b>, I still need to check other people's welfare since I'm also part of Membership committee which is akin to Internals in DVUP.
                For <b>UP CSI</b>, I've gotta contact alumni regarding requesting for academic resources. 
                    Additionally, I need to contribute to a few PRs and catch up in the Dev Camp.
                For <b>Toss UP</b>, I'm on track although we're gonna be having a catch-up meeting relatively soon for one of our events.
            Send help. <span><i class="fa-solid fa-face-sad-cry"/></span>
        </svelte:fragment>
    </AccordionItem>
    <AccordionItem>
        <svelte:fragment slot="lead"><i class="fa-solid fa-bed"/></svelte:fragment>
        <svelte:fragment slot="summary">
            Have you been able to take some time off for yourself recently? 
            What are the ways in which you relax/reduce stress?
        </svelte:fragment>
        <svelte:fragment slot="content">
            Yep, definitely. 
                Practically the entire Holy Week has been dedicated to me, myself, and I. 
                    For one thing, I finally finished my computer build since my GPU arrived the week prior while I was at my dorm.
                        So of course I had a bit of fun with that while it was still brand, spankin' new.
                    Other than that, I've mostly just been playing Terraria and some other games that I haven't played in a while (e.g., Lethal Company).
                    Star Rail has also been my bread-and-butter and when I'm at school.
                Another thing I generally do when I'm home is hang out with my little sister and pet dogs. 
                    They both do deserve some love and attention every now and then, and I'm here to provide.
        </svelte:fragment>
    </AccordionItem>
    <AccordionItem open>
        <svelte:fragment slot="lead"><i class="fa-solid fa-users"/></svelte:fragment>
        <svelte:fragment slot="summary">Anything we can do at Internals or for DevelUP as a whole to help you out?</svelte:fragment>
        <svelte:fragment slot="content">
            I mean, I'm an Internals person too. 
            But yeah, you guys have been doing great so far!
            Honestly, a couple more hangouts and events may be nice for the mems to get to know each other. 
                Maybe a couple more Jackbox or whatever game nights could be in order...?
            Nevertheless though, I think you guys are doing great! 
                Keep up the great work. <span><i class="fa-solid fa-hand-fist"/></span>
        </svelte:fragment>
    </AccordionItem>
    <!-- ... -->
</Accordion>