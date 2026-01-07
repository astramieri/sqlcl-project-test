# SQLcl commands

### 0. Connect in `thin` mode

    sql -thin hr/Oracle01@pdb1

### 1. Initialize SQLcl project

    SQL> project init -name <project> -schemas <schema>

### 2. Export DB objects

    SQL> project export

### 3. "Copy" everything from `src` to `dist`

This will generate the scripts and Liquibase changelogs for the brach.

    SQL> project stage