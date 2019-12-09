<script>
    export let firstName;
    export let lastName;
    export let email;
    export let phoneNumber;
    export let socialMedia;
    export let professionalSummary;
    export let experience;
    export let keyProjects;
    export let education;

	export const resume = undefined;
</script>

<div id="resumeContainer" class="c14 c18">
      <p class="c31"><span class="c24 c16 c27">{firstName}<span class="c24 c27 c16">&nbsp;{lastName}</span></p>
      <p class="c1"><span class="c12 c34"><a class="c7" href="mailto:{email}">{email}</a></span><span class="c12">&nbsp;| </span><span class="c16 c12">{phoneNumber}</span><span class="c6 c4">&nbsp;</span></p>
      <p class="c1">
	  	{#each socialMedia as socialMediaLink, index}
		<span class="c25 c14 c12">
            <a class="c7" href="{socialMediaLink}">{socialMediaLink}</a>
		</span>
			{#if socialMedia.length != (index + 1)}
			<span class="c12"> | </span>
			{:else}
			<span class="c6 c12 c32">&nbsp;</span>
			{/if}
		{/each}
      </p>
      <h1 class="c29"><span class="c24 c11 c16">PROFESSIONAL SUMMARY</span></h1>
      <ul class="c23 lst-kix_list_14-0 start">
	  	{#each professionalSummary as item, index}
		<li class="c17 c5">
            <span class="c14 c12">
              {item.skill}
			  {#each item.bolded as itemBolded, i}
			  	<span class="c8 c4">{itemBolded}</span>
			  	{#if item.bolded.length != (i + 1)}
				<span class="c3 c4">, </span>
				{:else}
				<span class="c3 c4"></span>
				{/if}
			  {/each}
            </span>
          </li>
		{/each}
      </ul>
      <h1 class="c19"><span class="c24 c11 c16">EXPERIENCE</span></h1>
		{#each experience as item, index}
			<p class="c1"><span class="c24 c4 c16">{item.jobTitle} | {item.role} | {item.duration}</span></p>
			<p class="c1"><span class="c12 c37">{item.summaryOfCompany}</span></p>
			<ul class="c23 lst-kix_list_2-0 start">
			{#each item.bulletsOfRole as itemBullets, i}
				<li class="c0"><span class="c6 c4">{itemBullets}</span></li>
			{/each}
			</ul>
		{/each}
      <h1 id="page-break-1" class="c19"><span class="c24 c11 c16">KEY PROJECTS</span></h1>
	  	{#each keyProjects as item, index}
			<p class="c10"><span class="c24 c4 c16">{item.role} (Client: {item.projectName})</span></p>
        	<ul class="c23 lst-kix_list_2-0">
			{#each item.bulletsOfRole as itemBullets, i}
				<li class="c0"><span class="c6 c4">{itemBullets}</span></li>
			{/each}
			</ul>
		{/each}
      <h1 class="c19" id="h.aljsgaeh8u18"><span class="c24 c11 c16">EDUCATION</span></h1>
	  	{#each education as item, index}
			<p class="c1"><span>{item.schoolName} &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{item.yearCompleted}<br>{item.educationCompleted}</span></p>
		{/each}
      <div>
          <p class="c33 c35"><span class="c6 c11"></span></p>
      </div>
    </div>

<style>
  
  .c29 {
      padding-top: 14pt;
      border-top-width: 3pt;
      border-bottom-color: #7f7f7f;
      padding-bottom: 5pt;
      line-height: 1.0;
      page-break-after: avoid;
      border-top-style: solid;
      border-bottom-width: 1pt;
      border-top-color: #262626;
      border-bottom-style: solid;
      orphans: 2;
      widows: 2;
      text-align: left
  }
  
  .c19 {
      padding-top: 5pt;
      border-top-width: 3pt;
      border-bottom-color: #7f7f7f;
      padding-bottom: 5pt;
      line-height: 1.0;
      page-break-after: avoid;
      border-top-style: solid;
      border-bottom-width: 1pt;
      border-top-color: #262626;
      border-bottom-style: solid;
      orphans: 2;
      widows: 2;
      text-align: left
  }
  
  .c0 {
      margin-left: 18pt;
      padding-top: 0pt;
      padding-left: -7.2pt;
      padding-bottom: 6pt;
      line-height: 1.3;
      orphans: 2;
      widows: 2;
      text-align: left
  }
  
  .c10 {
      margin-left: 10.8pt;
      padding-top: 0pt;
      text-indent: -10.8pt;
      padding-bottom: 6pt;
      line-height: 1.3;
      orphans: 2;
      widows: 2;
      text-align: left
  }
  
  .c22 {
      padding-top: 0pt;
      text-indent: -10.5pt;
      padding-bottom: 6pt;
      line-height: 1.3;
      orphans: 2;
      widows: 2;
      text-align: left
  }
  
  .c31 {
      padding-top: 0pt;
      padding-bottom: 9pt;
      line-height: 1.0;
      orphans: 2;
      widows: 2;
      text-align: left
  }

  .c8 {
    font-weight: 700;
    text-decoration: none;
    vertical-align: baseline;
    font-family: "Tahoma";
    font-style: normal
}
  
  .c3 {
      font-weight: 400;
      text-decoration: none;
      vertical-align: baseline;
      font-family: "Tahoma";
      font-style: normal
  }
  
  .c35 {
      padding-top: 12pt;
      padding-bottom: 0pt;
      line-height: 1.0;
      orphans: 2;
      widows: 2;
      text-align: left
  }
  
  .c17 {
      padding-top: 0pt;
      padding-bottom: 0pt;
      line-height: 1.3;
      orphans: 2;
      widows: 2;
      text-align: left
  }
  
  .c1 {
      padding-top: 0pt;
      padding-bottom: 9pt;
      line-height: 1.3;
      orphans: 2;
      widows: 2;
      text-align: left
  }

.c6 {
    font-weight: 400;
    text-decoration: none;
    vertical-align: baseline;
    font-family: "Tahoma";
    font-style: normal
}

.c25 {
    text-decoration-skip-ink: none;
    -webkit-text-decoration-skip: none;
    color: #1155cc;
    text-decoration: underline
}

.c34 {
    text-decoration-skip-ink: none;
    -webkit-text-decoration-skip: none;
    color: #53c3c7;
    text-decoration: underline
}

.c24 {
    text-decoration: none;
    vertical-align: baseline;
    font-family: "Tahoma";
    font-style: normal
}

.c7 {
    color: inherit;
    text-decoration: inherit
}


.c18 {
    max-width: 500.2pt;
    padding: 44.8pt 33.5pt 52pt 33.5pt
}

.c23 {
    padding: 0;
    margin: 0
}

.c5 {
    margin-left: 20pt;
    padding-left: 0pt
}

.c4 {
    color: #7f7f7f;
    font-size: 9pt
}

.c11 {
    color: #0e0b05;
    font-size: 12pt
}

.c27 {
    color: #0e0b05;
    font-size: 30pt
}

.c33 {
    height: 10pt
}

.c37 {
    font-style: italic
}

.c16 {
    font-weight: 700
}

.c32 {
    color: #000000
}

.c12 {
    font-size: 9pt
}

li {
    color: #7f7f7f;
    font-size: 10pt;
    font-family: "Tahoma"
}

p {
    margin: 0;
    color: #7f7f7f;
    font-size: 10pt;
    font-family: "Tahoma"
}

h1 {
    padding-top: 5pt;
    color: #0e0b05;
    border-top-width: 3pt;
    border-bottom-color: #7f7f7f;
    font-weight: 700;
    font-size: 12pt;
    padding-bottom: 5pt;
    line-height: 1.0;
    page-break-after: avoid;
    border-top-style: solid;
    border-bottom-width: 1pt;
    border-top-color: #262626;
    font-family: "Tahoma";
    border-bottom-style: solid;
    orphans: 2;
    widows: 2;
    text-align: left
}

@media print {
    #page-break-1 {
        page-break-before: always;
    }
  }

@media only screen and (max-width: 600px) {
    .c18 {
        max-width: 500.2pt;
        padding: 54.8pt 43.2pt 62pt 48.5pt
    }
}
</style>