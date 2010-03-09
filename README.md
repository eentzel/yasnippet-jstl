A collection of snippets I've found useful while editing JSP files
using emacs & [yasnippet mode](http://code.google.com/p/yasnippet/).
Covers a subset of the [core JSTL
tags](http://java.sun.com/products/jsp/jstl/1.1/docs/tlddocs/c/tld-summary.html).
Assumes that you use a mode called "jsp-mode" to edit JSPs.  If this
isn't true, you can either rename the jsp-mode directory to the name
of the mode you use, or you can put something like this in your .emacs
(assuming you currently use nxhtml-mode to edit JSPs):

    (define-derived-mode jsp-mode nxhtml-mode "JSP"
      "Major mode for editing .jsp files - identical to nxhtml-mode, but
      allows some mode hooks to run for jsp-mode but not html-mode")
    (add-to-list 'auto-mode-alist '("\\.jsp$" . jsp-mode))

If you make any additions or improvements to these snippets, pull
requests are welcome.