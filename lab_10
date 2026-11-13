square(S, A, Peri) :-
    A is S * S,
    Peri is 4 * S.


rectangle(L, W, A, Peri) :-
    A is L * W,
    Peri is 2 * (L + W).


triangle(Base, H, S1, S2, Area, Peri) :-
    Area is (Base * H) / 2,
    Peri is Base + S1 + S2.




validUser(sara, 1234).
validUser(ahmed, 2233).
validUser(Chloe, 4321).



login :-
    loginAttempts(3).



loginAttempts(0) :-
    write('Sorry, you exceeded the maximum number of attempts, try again later.').

loginAttempts(Attempts) :-
    Attempts > 0,
    write('Enter username: '),
    read(Username),
    write('Enter password: '),
    read(Password),
    (
        validUser(Username, Password)
        ->
        write('Login Successful!')
        ;
        write('Login Unsuccessful!'),
        nl,
        NewAttempts is Attempts - 1,
        loginAttempts(NewAttempts)
    ).
