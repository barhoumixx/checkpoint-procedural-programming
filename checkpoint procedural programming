FUNCTION scalar_prod(a: ARRAY_OF INTEGER,b: ARRAY_OF INTEGER) : FLOAT
VAR
    ps:FLOAT:=0; //Contains the dot(scalar) product of v1 and v2 (vectors of IR)
BEGIN
    FOR i FROM 0 TO a.length-1 STEP 1  DO
        //dot product of 2 vectors: a = [a1, a2, …, an] and b = [b1, b2, …, bn] is a.b = a1*b1 + a2*b2 +....+ an*bn
        ps:=ps+a[i]*b[i];
    END_FOR
    RETURN ps ;
END
//********
ALGORITHM scalar_product_of_vectors
VAR
    V1:ARRAY_OF INTEGER[3]; V2:ARRAY_OF INTEGER[3];
    x:FLOAT;
BEGIN
//Lire les deux vecteurs
    Write("Donner les 3 composantes du 1er vecteur")
    FOR i FROM 0 TO V1.length-1 DO
        Write("Composante", i ); Read(V1[i]);
    END_FOR
    Write("Donner les 3 composantes du 2eme vecteur")
    FOR i FROM 0 TO V2.length-1 DO
        Write("Composante", i ); Read(V2[i]);
    END_FOR
//Appel à la fonction
    x:= dot_product(V1,V2);
    IF (x=0) THEN
        Write("The dot product of the vectors is zero. They are orthogonal.")
    ELSE
        Write("The vectors are not orthogonal.")
    END_IF
END
10 h 07
PROCEDURE insertion_sort(VAR arr : ARRAY_OF INTEGER)
VAR
   n,i,j,tmp : INTEGER;
BEGIN
   n := arr.length;
   FOR i FROM 0 TO n DO
      tmp:=arr[i]; //We stock arr[i] in tmp in order not to lose it when we move the elements
      j := i - 1; //Each time work only with the first i-1 element from of the array
        /* Move the elements of arr, that are greater than arr[i] (stored in tmp), to one position ahead of their current one */
        WHILE (j >= 0 and arr[j] > tmp) DO
            arr[j + 1] := arr[j]; //swap the elements if tmp<arr[j]
            j := j - 1;//decrease j to continue comparing with the sorted elements
        END_WHILE
        arr[j + 1] = tmp; // insert tmp (arr[i]) into its place in the sorted sequence in the array
   END_FOR
END
/* *** Insertion Sort Algorithm *** */
ALGORITHM InsertionSort
VAR
    n,i:INTEGER;
    V1:ARRAY_OF INTEGER[n];
BEGIN
    //Read the array
    Write("Give the length of the array") ; Read(n);
    Write("Give the elements of the array")
    FOR i FROM 0 TO n-1 DO
       Read(V1[i]);
    END_FOR
    Write("the original unsorted array",V1) ;
    //Sort the array
    insertion_sort(V1,n);
    //Display the sorted array
    Write("the final sorted array",V1) ;
END
coche_blanche
yeux
alléluia























