Download Link: https://assignmentchef.com/product/solved-cpe212-project04
<br>
<strong>                </strong>

<h1>Project04 Description</h1>

<strong><em>Complete</em></strong>    the      provided        partial C++     program         that     will      implement     a          <strong><em>Priority          Queue ADT</em></strong><strong><em>    (abstract        data    type)</em></strong>   in         which  the      internal          representation           of         the      priority           queue is         a        doublelinked  series  of         dynamically   allocated         nodes.

The  <strong><em>Priority          Queue </em></strong>will      be        used    to         store   text     messages        read    from    an        input   file.                  Each        message         has      a          priority           (<strong>H</strong>        for       <strong>H</strong>igh,   <strong>M</strong>         for       <strong>M</strong>edium,         <strong>L</strong>          for       <strong>L</strong>ow).              When        input   from    the      file       by        the      <strong>main()</strong>           function,         the      message         and      priority           information    are        stored within an        object  of         the      type    <strong>Message</strong>.                    The     text     message         is         stored as        a        <strong>string</strong> attribute,        and      the      message         priority           is         represented   by        an        attribute         with    type        <strong>Priorities</strong>,      an        enumerated   type    provided.

<strong><em>Priority      Queue</em></strong> <strong>Rules  of        Operation</strong><strong>:</strong>

<ul>

 <li>If the      <strong><em>Priority          Queue</em></strong> contains          messages        which  have    different         priority           levels, then    the        highest           priority           messages        must   be        removed         from    the      FRONT            of         the      <strong><em>Priority        Queue</em></strong> before any      lower  priority           messages        are      removed         whenever       the      <strong>Dequeue()</strong>    method           is                             <strong>            </strong></li>

</ul>

<strong>HINT:          </strong>            The     priority           queue is         sorted by        Priority           Level   (highest          to         lowest)           as        it          is         being   constructed    by        <strong>Enqueue()</strong><strong>     </strong>in         much  the      same   way     as        we       discussed       with        the      implementation         of         a          sorted linked list.

<ul>

 <li>Given two     messages        of         the      <strong>same</strong>  priority           level,   the      message         that     has      been    in         the        <strong><em>Priority          Queue</em></strong> for       the      <strong>longest           time</strong>    has      the      highest                                 (FIFO  operation        within a          priority           level).<strong>  </strong></li>

</ul>

<strong>HINT:</strong>                                  A         new     message         of         a          given   priority           level    must   always be        added        AFTER any      other   messages        with    that     same   priority           level    that     were   already           in         the        <strong><em>Priority          Queue.</em></strong>

Between      the      lecture notes   and      textbook,        we       have    already           reviewed        much  of         the      source code    that        may     be        adapted          to         implement     the      <strong><em>Priority          Queue</em></strong> operations,     but      you      will      need    to        modify            this      code    to         complete        this      assignment.                Two    of         the      key      modifications will      be        the      addition          of         the      specified         exception       detection/handling   and      the      “previous”      links.               The        other   modification  requires          you      to         adapt  the      container        code    to         store   a          User-Defined Data        Type   (of       type    <strong>Message).</strong>

Additional   details may     be        found  on        subsequent    pages  of         the      handout.<strong><em>         </em></strong>

<h1>Running the Sample Solution on blackhawk</h1>

<strong><em>The  best     description    of         what   your    code    must   do        is         the      </em></strong><strong><em>Sample           Solution</em></strong><strong><em>         for       the      project.</em></strong>

Run the      sample            solution          by        typing the      following        at         <strong>blackhawk</strong>    terminal         window          command        prompt           where <strong>inputfilename</strong>     is         the      name   of         one      of         the      provided        input   files     (for        example,         <strong><em>p04input1.txt</em></strong>).




<strong>/home/work/cpe212/project04/p04   inputfilename </strong>




Your current           working          directory        must   contain           the      input   files     for       this      to         work.

<h1>Unzipping Sample Input Files on blackhawk</h1>

Use  the      Firefox            browser          to         access Canvas            and      download       <strong>main.cpp</strong>       and      the      sample        input   files     into     your    <strong>Project04</strong>      directory.                   At        terminal         window          prompt,          use      the        unzip  utility  to         uncompress   the      files.                For      example,         to         unzip  the      files     into     your    current        directory:

<strong>unzip  Project04_Materials.zip </strong>

Since            this      project            is         worth  five      points, you      have    been    given   three   input   files     to         test      your        program.

<h1>Running the Preview Script on blackhawk</h1>

Preconditions         for       running          the      Preview          script:

<ul>

 <li><strong><em>Your current          working         directory       must   contain          both    your    </em></strong><strong><em>project04</em></strong><strong><em>       executable     and     all  sample           input  files</em></strong><strong><em>     </em></strong><strong><em>BEFORE</em></strong><strong><em>          you     execute          the      preview          script!!!          </em></strong></li>

 <li>Linux is         case     sensitive         –          be        sure    the      name   of         your    executable      is                                 <strong><em>project04</em></strong></li>

</ul>




Run  the      preview          script  by        typing the      following        in         a          <strong>blackhawk</strong>    terminal         window          command        prompt

<strong>/home/work/cpe212data/project04/preview04.bash     </strong>




This script  will      run      both    the      Sample           Solution          AND    your    project04       executable      program         on        the        complete        set       of         input   files,    and      it          compares       the      outputs           of         the      two     programs       line        by        line      to         identify           errors in         your    program’s      outputs.                      Make   sure    that     the      output of        your    program         exactly            matches          the      output of         the      Sample           Solution.

<strong><em>Be    sure    to        fix        any     </em></strong><strong><em>memory         leaks</em></strong><strong><em>   identified       by        the      preview          script  to        receive           full        credit. </em></strong>

<strong><em>        </em></strong>

<strong>Project04 Files Provided – DO </strong><strong>NOT</strong><strong> MODIFY OR SUBMIT THESE FILES </strong><strong>**</strong> <strong> </strong><strong>priorityq.h</strong>        –               declares                 the           <strong><em>Priority             Queue   ADT</em></strong>        class       and         describes              its            member                functions<strong>              message.h</strong>          –               declares                 the             <strong>Message</strong>               class,      the           type        of              data        stored   in              each       <strong><em>Priority                 Queue   </em></strong>node.<strong>     main.cpp</strong>             –             includes                 the           <strong>main()</strong> function                 test         driver    for           the           <strong><em>Priority                 Queue</em></strong>   class.<strong>      </strong>

<strong>makefile</strong>             –            includes                 all             commands           required                to             compile                  and         link         your       project  on              <strong><em>blackhawk</em></strong><strong><em>         Do            not          modify or             submit </em></strong><strong><em>any         of             the          provided              files        named above</em></strong><strong><em>**</em></strong><strong><em>              </em></strong><strong><em>!!!</em></strong>             <strong><em>                  </em></strong><strong><em>                  </em></strong>




<strong>         add         your      code      here       to             implement         the             member               function               of             the          </strong><strong>Message</strong><strong>               class.</strong><strong>     priorityq.cpp   </strong><strong>–               add         your      code      here       to             implement         </strong><strong>PriorityQ</strong><strong>            functionality                                        </strong>

<strong>The   code      in             </strong><strong>message.cpp</strong><strong>    and         </strong><strong>priorityq.cpp</strong><strong>   must      not          include                 any         INPUT  or             OUTPUT               statements.                    </strong>

<strong>PRINT               functions             have      been      included              in             </strong><strong>message.h</strong><strong>          and         </strong><strong>priorityq.h</strong><strong>         for           debugging          purposes                                            <em>Use         of             the          Standard             Template             Library                  containers          or             container            adapters              is              not             allowed.                                                    </em></strong>




<strong>How to get started on this assignment? </strong>

<strong>See  </strong><strong>message.h</strong><strong>     and     </strong><strong>priorityq.h</strong><strong>    for       descriptions of        </strong><strong>Message        ADT</strong><strong>    and     </strong><strong>PriorityQ       ADT</strong><strong>.   </strong>

<strong>Once           again, I           recommend  creating         an       </strong><strong>Empty Framework  of        function         definitions</strong><strong>    </strong><strong>in             </strong><strong>message.cpp</strong><strong>    and         </strong><strong>priorityq.cpp</strong><strong>  that     compiles       first    –          before            adding           any     code   to        any        function.        </strong>

<strong>Complete   the      entire </strong><strong>Message        ADT    </strong><strong>first    and     then    address         the      critical           operations    within        </strong><strong>PriorityQ       </strong><strong>functions       [           </strong><strong>constructor, Enqueue(),    Dequeue()    </strong><strong>]</strong><strong>                       </strong><strong>since  these  critical           items        must   be        functional     in        order  to        test     other  operations.               </strong><strong>            </strong>

<strong>Make           sure    these  critical           operations    work  before            adding           code   for       any     non-critical        operations.</strong><strong>   </strong>




<h1>Program Compilation Instructions</h1>

This project            consists          of         two     C++     files     provided        by        the      instructor,      along   with    a          file        named <strong>makefile</strong>        to         help     you      compile          your    program.                    So,       for       this      assignment,    all        you        must   do        to         compile          the      program         is         to         use      the      following        command       at         the        Linux  command       line      <strong>make  </strong>which  will      create an        executable      named            <strong>project04</strong>      from    the      provided        files.




If      your    program         compiled        successfully,   you      may     then    type

<strong>./project04                                    NameOfInputFile     </strong>to         execute           your    program         assuming        that     the      input        file       is         located            in         the      same   directory        with    the      executable.





