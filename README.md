Simple port of the code in 'Manuale di Programmazione Cinematografica' by Daniele Olmisani from Processing to p5.js. The original code (i.e. '.pde' files) is found in a github repository @ https://github.com/mad4j/book-mdpc.  Each sketch represents a 'Minimalist movie poster' of a well known movie.  At the moment there are 110 films in all.

Because of various size restrictions, all of the p5.js renditions of the sketches are provided in a single zip file that contains:

<ul>
<li><i>html files and an index file</i> -- There is one html file for each sketch. The html file delineates required libraries, as well as a link to a specific sketch name. Additionally, there is an index html file that provides links to all of the sketches associated with the book (via the html files).</li>
<li><i>p5progs subdirectory</i> -- This subdirectory contains all of the sketches for a particular book title. The basic structure of the sketch name is 'sketch-<abbrev book title>-<chapter and section>_<short_description>.js'. The chapter and section designations depend on the specific book. For example, 'sketch-ddgd-ch4_e_AnimatingText.js' refers to the 4th chapter - section 'e' of Data Driven Graph Design. The sketch deals with animated text.</li>
<li><i>p5libs subdirectory</i> -- These are the p5.js libraries used (collectively) by the sketches.</li>
<li><i>data subdirectory</i> -- These are the data files or assets used collectively by the sketches.</li>
<li><i>tn_images subdirectory</i> -- These are thumbnails produced from the screen shots that are produced individually from the sketches. If you want a different screen shot, then the output of a sketch can be saved by simply typing 's' or 'S' after the sketch has been loaded.</li>
</ul>

I should note there is a bit of 'hard coding' in the 'index' file. If you look at the file, you'll see 'a href' links of the following sort:

"http://localhost/Cinematographica/Cinematographica-sketch-vol1-alice_in_wonderland.html"

Here, the link is being executed via a 'localhost' setup where 'Cinematographica/' is a top-level subdirectory containing the files and structure noted above.  If you want to use the index file with another setup up, then you'll probably use a global edit to replace 'localhost' in the index.html with the appropriate server designation(s). Additionally, you can easily shift out the top-level subdirectory.  However, other changes to the structure are likely to be a little more onerous. For instance, changing the 'p5progs/', 'p5libs/' and 'data'/ subdirectory names would require a substantial change to all of the html files and in the case of the 'data' subdirectory to many of the sketches.
