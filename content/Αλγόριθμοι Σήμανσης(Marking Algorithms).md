
## Αλγόριθμοι Σήμανσης

Οι αλγόριθμοι σήμανσης για την επίλυση του προβήματος της κρυφής μνήμης είναι μια κλάση αλγορίθμων οι οποίοι περιγράφονται από τον παρακάτω ψευδοκώδικα:

$$

\begin{align}\\ 
& \text{Κάθε στοιχείο μνήμης είναι είτε \textbf{marked} ή \textbf{unmarked}}\\ 
&\text{Στην αρχή όλα τα στοιχεία είναι \textbf{unmarked}}\\ 
&\\
&\text{Σε ένα αίτημα του στοιχείου s:}\\
&  \; \; \; \text{\textbf{Σημειώνουμε(Mark)} το s}\\
&  \; \; \; \textbf{If } \text{s είναι στην cache} \; \textbf{then} \; \text{δεν απομακρύνεται κανένα στοιχείο}\\
&  \; \; \; \textbf{Else } \text{το s δεν είναι στην cache:} \\
&  \; \; \; \; \; \; \textbf{If } \text{όλα τα στοιχεία της cache είναι marked}  \\
&  \; \; \; \; \; \; \textbf{then} \\
&  \; \; \; \; \; \; \; \; \; \text{Ολοκληρώνεται η φάση}\\
&  \; \; \; \; \; \; \; \; \; \text{Η επεξεργασία του s μετατίθεται στην αρχή της επόμενης φάσης}\\
&  \; \; \; \; \; \; \textbf{Else } \text{απομακρύνεται \textbf{ένα unmarked στοιχείο} από την cache}  \\
&  \; \; \; \; \; \; \textbf{EndIf }  \\
&  \; \; \;  \textbf{EndIf }   \\
\end{align}

$$

$$
\begin{algorithm}

\caption{Cache Management Algorithm} \begin{algorithmic}[1] 

\STATE Κάθε στοιχείο μνήμης είναι είτε \textit{marked} ή \textit{unmarked} 

\STATE Στην αρχή όλα τα στοιχεία είναι \textit{unmarked} 
\FORALL{αίτημα του στοιχείου $s$} 
\STATE Σημειώνουμε (\textit{Mark}) το $s$ 
\IF{$s$ είναι στην \textit{cache}} 
\STATE δεν απομακρύνεται κανένα στοιχείο 
\ELSE \IF{το $s$ δεν είναι στην \textit{cache}} 
\IF{όλα τα στοιχεία της \textit{cache} είναι \textit{marked}} 
\STATE Ολοκληρώνεται η φάση 
\STATE Η επεξεργασία του $s$ μετατίθεται στην αρχή της επόμενης φάσης 
\ELSE \STATE απομακρύνεται ένα \textit{unmarked} στοιχείο από την \textit{cache} \ENDIF 
\ENDIF 
\ENDIF 
\ENDFOR 

\end{algorithmic} 

\end{algorithm}
$$

## Τυχαιοποιημένος Αλγόριθμος Σήμανσης



$$

\begin{align}\\ 
& \text{Κάθε στοιχείο μνήμης είναι είτε \textbf{marked} ή \textbf{unmarked}}\\ 
&\text{Στην αρχή όλα τα στοιχεία είναι \textbf{unmarked}}\\ 
&\\
&\text{Σε ένα αίτημα του στοιχείου s:}\\
&  \; \; \; \text{\textbf{Σημειώνουμε(Mark)} το s}\\
&  \; \; \; \textbf{If } \text{s είναι στην cache} \; \textbf{then} \; \text{δεν απομακρύνεται κανένα στοιχείο}\\
&  \; \; \; \textbf{Else } \text{το s δεν είναι στην cache:} \\
&  \; \; \; \; \; \; \textbf{If } \text{όλα τα στοιχεία της cache είναι marked}  \\
&  \; \; \; \; \; \; \textbf{then} \\
&  \; \; \; \; \; \; \; \; \; \text{Ολοκληρώνεται η φάση}\\
&  \; \; \; \; \; \; \; \; \; \text{Η επεξεργασία του s μετατίθεται στην αρχή της επόμενης φάσης}\\
&  \; \; \; \; \; \; \textbf{Else } \text{απομακρύνεται \textbf{ένα τυχαίο unmarked στοιχείο ομοιόμορφα στην τύχη} από την cache}  \\
&  \; \; \; \; \; \; \textbf{EndIf }  \\
&  \; \; \;  \textbf{EndIf }   \\
\end{align}

$$