# YouTube-Channel-Scrapper
YouTube Channel All Videos Info like Name, Views &amp; Link


How to Get/Export/Copy/Extract Titles, URLs and Views of any YouTube Channel without needing to install anything and just using your browser. This can video can help you a lot in order to extract all titles, URLs and views of the YouTube videos from any channel

Console of Browser

🔷 Step 1:
`var scroll = setInterval(function(){ window.scrollBy(0, 1000)}, 1000);`

🔷 Step 2:
`window.clearInterval(scroll); console.clear(); urls = $$('a'); urls.forEach(function(v,i,a){if (v.id=="video-title-link" && v.href){console.log('\t'+new Date().toLocaleDateString()+'\t'+v.title+'\t'+v.href+'\t'+v.__shady_native_innerHTML.match(/aria-label=\"(.+?)\"/g)?.[0].match(/[\d,]+ views/g)[0]+'\t')}});`
