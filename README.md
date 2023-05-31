# BD-P3-CASO-7
1*) A= ρ N ← nom,T ← titulo Actua
    B= A ⨯ Actua
    π nom (σ N = nom ∧ T ≠ titulo B)
2*) Persona ⨝ (π nom Actua ⨝ π nom Dirige)
3*) Persona ⨝ (π nom Actua - π nom Dirige)
4*) A= π titulo σ nom='Carrie-Anne Moss' Dirige
    Persona ⨝ (Actua ÷ A)
5*) A= π titulo σ nom= 'Keanu Reeves' Dirige
    π titulo,estreno (Pelicula ⨝ A)
6*) A= π titulo σ nom='Keanu Reeves' Actua
    σ nom ≠ 'Keanu Reeves' Actua ÷ A
7*) si es todas las peliculas*) A= π titulo σ nom='Keanu Reeves' Actua
                                B= π nom (σ nom ≠ 'Keanu Reeves' Dirige ÷ A)
                                C= π nom (σ nom ≠ 'Keanu Reeves' Actua ÷ A)
                                Persona ⨝ (B ∪ C)
    si es por lo menos una pelicula*) A= π titulo σ nom='Keanu Reeves' Actua
                                      B= π nom (σ nom ≠ 'Keanu Reeves' Dirige ⨝ A)
                                      C= π nom (σ nom ≠ 'Keanu Reeves' Actua ⨝ A)
                                      Persona ⨝ (B ∪ C)
8*) π nom (σ titulo='The Matrix' Actua) ∩ π nom (σ titulo='The Matrix Revolutions' Actua)
9*) A= π nom σ titulo ≠ 'The Matrix Revolutions' Actua
    π nom Actua - A
10*) π nom (Persona ⨝ (ρ nom ← seguidor Sigue))
11*) π nom (Persona ⨝ (ρ nom ← seguidor (π seguidor σ seguido = 'George Martin' Sigue) ∩ (π seguidor σ seguido = 'Keanu Reeves' Sigue)))
