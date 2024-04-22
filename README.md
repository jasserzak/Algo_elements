ALGORITHM sentence
VAR 
    c:CHAR;
    nbrC,nbrV,nbrW:INTEGER;
BEGIN
    nbrC := 0
    nbrV := 0
    nbrW := 0
    REPEAT
      Read(c); 
      nbrC := nbrC+1
      IF (c= 'a'OR c='e'OR c='u'OR c='o'OR c='i'OR c='y') THEN
      nbrV := nbrV+1
      END_IF
      IF (c=' ' OR c='.') THEN
      nbrW := nbrW+1
      END_IF
    UNTIL (c='.')
    Write("nombre totale de caractères:",nbrC)
    Write("nombre totale de mots:",nbrC)
    Write("nombre totale de voyelles:",nbrC)
END
