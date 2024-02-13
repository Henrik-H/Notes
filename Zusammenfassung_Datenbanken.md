
# Skalierung

- Horizontale Skalierung - NoSql
- Vertikale Skalierung - Sql

# 3 V's

- Data Velocity
- Data Variety
- Data Volume

# 3 Aufgabenbereiche

| acronym | meaning | examples |
| ---- | ---- | ---- |
| DDL | Data Definition Language | CREATE, DROP |
| DML | Data Manipulation Language | SELECT, UPDATE |
| DCL | Data Control Language | GRANT, REVOKE |

# CRUD

| Operationen | SQL-Befehle |
| ---- | ---- |
| Create | INSERT |
| Read | SELECT |
| Update | UPDATE |
| Delete | DELETE |

# CAP-Theorem

> Das CAP-Theorem besagt, dass ein verteiltes Datenbanksystem nur zwei von den drei Eigenschaften gleichzeitig gewährleisten kann.

- Konsistenz (alle Knoten sehen die gleichen Daten zur gleichen Zeit)
- Verfügbarkeit (alle Anfragen erhalte eine Antwort)
- Partitionstoleranz (das System funktioniert trotz Netzwerkausfällen)

>Partitationstoleranz ist meist notwending (nicht optional)

- CP ( starke Konsistenz )
- AP ( starke Verfügbarkeit )

# ACID
- Atomic
- Consistent
- Isolated
- Durable

# BASE
 - Basically available
 - Soft state
 - Eventually consitent

# Normalform

1NF keine zusammengesetzte Werte
2NF Nicht-Key Werte müseen von dem **gesamten** Schlüssel abhängen also bei zusammengesetzten Schlüsseln nicht nur von einem
3NF Attribute dürfen nicht voneinander ableitbar sein

# Keys

- Primärschlüssel 
	ausgewählter Schlüsselkandidat, der zur eindeutigen Identifikation jedes Datensatzes in der Tabelle verwendet wird.
- Fremdschlüssel
	ein Attribut oder eine Attributkombination in einer Tabelle, die auf den Primärschlüssel einer anderen Tabelle verweist und dadurch eine Beziehung zwischen den Tabellen herstellt.
- Schlüsselkanidat
	Ein Schlüsselkandidat ist eine Kombination von Attributen, die einen Datensatz eindeutig identifizieren können. In einer Tabelle kann es mehrere Schlüsselkandidaten geben.

# Where

```SQL
--- BETWEEN AND
WHERE column_name BETWEEN value1 AND value2;

--- LIKE
WHERE column_name LIKE 'Text_gesucht';
WHERE column_name LIKE 'A%l'; --- Fängt mit A an, endet mit l
WHERE column_name LIKE 'Apfe_'; --- Zeichen vor oder nach dem Text

--- IS NULL
WHERE column_name IS NULL;
WHERE column_name IS NOT NULL;
```

# Joins

INNER JOIN = $A \cap B$

LEFT JOIN = $A$

OUTER JOIN = $A \cup B$


