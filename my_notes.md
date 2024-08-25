# Run venv
pandas_workshop\Scripts\activate

# How melt works

tsa_melted = tsa.melt(
    id_vars='date',        # Kolumna, która pozostaje nienaruszona i identyfikuje unikalne wiersze
    var_name='year',       # Nazwa nowej kolumny, która będzie zawierać dawną nazwę kolumny (2019, 2020, 2021) -> przekształcenie nazw kolumn które nie są identyfikatorami na wartości w nowej kolumnie o podanej nazwie
    value_name='travelers' # Nazwa nowej kolumny, która będzie zawierać wartości (liczba podróżnych) -> nazwa nowej kolumny która będzie zaweirała wartości z kolumn które nie są identyfikatorami
)

# NEXT
5. Time series