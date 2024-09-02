<script>
    import { dues } from '$lib/utils/helper';
    let one, oneOne, oneOneOne, oneTwo, oneTwoOne, oneTwoTwo, oneTwoThree, oneTwoFour, oneTwoFive, oneThree;
    let two, twoOne, twoTwo, twoThree;
    let three, threeOne;
    let four, fourOne, fourTwo;
    let five, fiveOne, fiveTwo;
    let six, sixOne, sixTwo, sixThree;
    let seven, sevenOne, sevenTwo, sevenThree;

    const goToSection = (section) => {
        const top = section.getBoundingClientRect().top + window.pageYOffset;
        window.scrollTo({left: 0, top, behavior: 'smooth'});
    }
</script>

<style>
    .constitution {
        position: relative;
        z-index: 1;
        width: 92%;
        max-width: 800px;
        margin: 8em auto 10em;
        color: #fff;
    }

    h1 {
        font-size: 2em;
        line-height: 1.2em;
        text-align: center;
        margin: 2em 0 1.5em;
    }

    h2 {
        font-size: 1.5em;
        line-height: 1.2em;
    }

    h3 {
        text-decoration: underline;
        font-size: 1.3em;
        line-height: 1.2em;
    }

    h4 {
        text-decoration: underline;
        margin-left: 2em;
        font-size: 1.2em;
        line-height: 1.2em;
    }

    h5 {
        margin-left: 6em;
        font-size: 0.8em;
        line-height: 1.1em;
    }

    .subBlock {
        margin-left: 2.4em;
    }

    .sectionHeading {
        margin: 4em 0 1.5em;
    }

    .subSectionHeading {
        margin: 1.5em 0 1.5em;
    }

    .underscore {
        text-decoration: underline;
    }

    .right {
        text-align: right;
    }

    .positionMaximums td {
        min-width: 3em;
    }

    .noUnderscore {
        text-decoration: none;
    }

    .clickable {
        cursor: pointer;
    }

    .clickable:hover {
        color: #00316b;
    }

    p, ul, li {
        color: #708090;
    }
</style>

<div class="constitution">
    <h1 class="noUnderscore">LEGENDS LEAGUE CONSTITUTION</h1>
    
    <h2 class="noUnderscore">TABLE OF CONTENTS</h2>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(one)}>Section 1: Roster Breakdown</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(oneOne)}>1.1 Positional Breakdown</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(oneTwo)}>1.2 Trading</h4>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(oneTwoOne)}>1.2.1 Trade Collusion</h5>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(oneTwoTwo)}>1.2.2 Lending Players Prohibition</h5>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(oneTwoThree)}>1.2.3 Trade Deadline</h5>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(oneTwoFive)}>1.2.5 Veto/Trade Process</h5>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(oneThree)}>1.3 Waiver Wire System</h4>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(two)}>Section 2: Drafting</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(twoOne)}>2.1 Keepers</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(twoTwo)}>2.2 Draft Order</h4>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(three)}>Section 3: Scoring System</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(threeOne)}>3.1 Scoring System</h4>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(four)}>Section 4: Postseason</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fourOne)}>4.1 Playoffs</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fourTwo)}>4.2 Seeding Tiebreakers</h4>

    <h3 class="noUnderscore clickable" on:click={() => goToSection(five)}>Section 5: Replacing Managers</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fiveOne)}>5.1 Removing Managers</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fiveTwo)}>5.2 Replacing Managers</h4>

    <h3 class="noUnderscore clickable" on:click={() => goToSection(six)}>Section 6: League Finances</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sixOne)}>6.1 League Dues</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sixTwo)}>6.2 Payout</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sixThree)}>6.3 Raising Dues</h4>
    
    <hr />
    
    <h2 class="sectionHeading" bind:this={one}>Section 1 Roster Breakdown</h2>
    
    <h3 class="subSectionHeading" bind:this={oneOne}>1.1 Positional Breakdown</h3>
    
    <p>28 Total Players</p>
    
    <p class="underscore">Starters</p>
    <ul>
        <li>QB</li>
        <li>RB</li>
        <li>RB</li>
        <li>WR</li>
        <li>WR</li>
        <li>WR</li>
        <li>TE</li>
        <li>FLEX (RB/WR/TE)</li>
        <li>K</li>
        <li>D/ST</li>
    </ul>
    
    <p>6 Bench</p>

    <p>1 IR Spot</p>
    
    <h3 class="subSectionHeading" bind:this={oneTwo}>1.2 Trading</h3>
    
    <p>Trades will occur per Sleeper App rules</p>
    
    <h4 bind:this={oneTwoOne}>1.2.1 Trade Collusion</h4>
    <div class="subBlock">
        <p>If any owners are suspected of accepting bribes/offering bribes to enhance their/another owners team via trade, trading any assets other than fantasy players, draft picks, FAAB $, or otherwise found guilty of engaging in any form of collusion*, all parties involved in the trade will be susceptible to punishment. The punishments will go as followed:</p>

        <p>All trades that are found guilty of collusion, will be reversed/denied. If the trade had affected the outcome of previous games, the results of those games will be revised.  </p>

        <p>*Collusion includes the organizing of veto votes against an acceptable trade.</p>

        <p>The commissioner will err on the side of letting owners manage their teams the way they see fit. Any collusion will need to be clear. The commissioner reserves the right to step in and at the very least assess the thinking of any team involved in a heavily lop-sided trade. </p>
    </div>

    <h4 bind:this={oneTwoTwo}>1.2.2 Lending Players Prohibition</h4>
    <div class="subBlock">
        <p>Any player traded from a team may not be re-acquired via trade within 6 weeks of the original trade. Any teams involved in this behavior will be subject to the aforementioned collusion punishments.</p>
    </div>
    
    <h4 bind:this={oneTwoThree}>1.2.3 Trade Deadline</h4>
    <div class="subBlock">
        <p>The trade deadline will be set for the Saturday of the week 11 games of the NFL season.</p>
    </div>
    
    <h4 bind:this={oneTwoFive}>1.2.5 Veto/Trade Process</h4>
    <div class="subBlock">
        <p>A total of 7 veto votes are required to veto a trade. Vetoes are only appropriate in instances of collusion or an egregious mismatch of value (i.e. CMC for a backup kicker). Not liking a trade does not warrant a veto.</p>
    </div>
    
    <h3 bind:this={oneThree}>1.3 Waiver Wire System</h3>
        <ol>
        <li>FAAB Waiver wire system.</li>
        <li>Each team will begin the season with $100.</li>       
        <li>$0 bids are allowed.</li>
        <li>Waivers clear Wednesday at 3AM Eastern.</li>
        <li>Players stay on the waivers for 2 days.</li>
        </ol>

    <h2 class="sectionHeading" bind:this={two}>Section 2 Drafting</h2>

    <h3 bind:this={twoOne}>2.1 Keepers</h3>
    <p>Each team is eligible to keep two players from their team's previous season roster, with the following stipulations</p>
        <ol>
            <li>Each team can keep up to two players every year.</li>
            <li>A keeper's draft position will be two rounds earlier than where they were drafted the previous year. For example, if a player was drafted in the 4th round the previous year, they will occupy a 2nd round slot in the year they are kept.</li>
            <li>Players cannot be kept if they were drafted in the first or second round the previous year.</li>
            <li>The original draft position is always used to determine keeper draft positions. For example, if a player was originally drafted, then dropped, and subsequently picked up and kept by another team, they will retain their original draft position when determing keeper rounds per #2.</li>
            <li>If a player was undrafted & picked-up during the season, they will be treated as a 10th round pick for keeper purposes, meaning they will occupy an 8th round slot in the following year's draft.</li>
            <li>Players picked up after the regular season cannot be kept.</li>
            <li>Players picked up during the playoffs (or after you were statistically eliminated if you didn’t make the playoffs) are ineligible to be kept.</li>
            <li>Keeper picks must be submitted at least 48 hours before draft day and time. No keeper decisions will be allowed after that.</li>
            <li>Extreme or rare circumstances, such as a season-ending injury in the 48-hour period, will be discussed on a case-by-case basis.</li>
            <li>A keeper can only be kept for 2 consecutive years; after that, they cannot be kept by the same owner.</li>
        </ol>

    <h3 bind:this={twoTwo}>2.2 Draft Order</h3>
    <p>The draft order each year will be a snake draft. Each year, one league member (excluding the commissioner) will be responsible for determining the draft order. This responsibility will rotate annually among all league members, so each member will have a turn to set the draft order.</p>
        <ul>
            <li>As an example, for the 2024 season, one member horrendously failed at this task by randomly assigning each league member a Men's 10km Olympic swimmer, but failed to take into consideration that the race took place at 1:30AM Eastern and several players would get COVID and not start or finish the race. Fortunately, other members of the league managed to salvage this error and determine an appropriate draft order.</li>
        </ul>
    <h2 class="sectionHeading" bind:this={three}>Section 3 Scoring System</h2>

    <h3 bind:this={threeOne}>3.1 Scoring System</h3>
    <p>The league scoring system breakdown is listed on the Sleeper fantasy app (for the most part, it follows typical .5PPR Scoring). The scoring system will never change without a majority league vote.</p>
    
    <h2 class="sectionHeading" bind:this={four}>Section 4 Postseason</h2>
    
    <h3 bind:this={fourOne}>4.1 Playoffs</h3>
        <ol>
        <li>At the end of the season, 6 teams will make the playoffs.</li>
        <li>Top two regular season teams receive a first-round Bye.</li>
        <li>The first round of playoffs will commence in week 15</li>
        <li>Each round will last one week.</li>
        <li>Week 18 will not be used.</li>
        </ol>
    
    <h3 bind:this={fourTwo}>4.2 Seeding Tiebreakers</h3>
    <p>Tiebreakers are determined per the following rules:</p>

    <ol>
        <li>Overall Record</li>
        <li>Points For</li>
        <li>Higher Points Against</li>
        <li>Coin Toss</li>
    </ol>
    
    <h2 class="sectionHeading" bind:this={five}>Section 5 Replace Managers</h2>
    <h3 bind:this={fiveOne}>5.1 Removing Managers</h3>
    <p>Short of continuously failing to set a valid lineup, or confirmed collusion, no manager can be removed against their will. Participation, through the league chat, trade offers, and the waiver wire, is strongly encouraged but generally grounds for removal.</p>
    
    <h3 bind:this={fiveTwo}>5.2 Replacing Managers</h3>
    <p>When a manager needs to be replaced, the commisiooners will try to find a suitable candidate with some connection to at least a portion of the existing managers. Priority will be placed on managers who are eager to take on a dynasty commitment and will be very active within the league.</p>
    
    <h2 class="sectionHeading" bind:this={six}>Section 6 League Finances</h2>
    
    <h3 bind:this={sixOne}>6.1 League Dues</h3>
    <p>League dues are set at {dues}$. Dues are required before the draft, otherwise your team will be set to auto-draft. </p>
    
    <h3 bind:this={sixTwo}>6.2 Payout</h3>
    <p>League payout is structured as follows:</p>
    <ul>
        <li>1st place: ${dues * 9}</li>
        <li>2nd place: ${dues * 1}</li>
    </ul>

    <h3 bind:this={sixThree}>6.3 Raising Dues</h3>
    <p>A ⅔ majority vote is required in order to raise league dues. In the event that a manager is no longer financially comfortable with the buyin, finding a co-manager to split the cost is reccomended.</p>

</div>