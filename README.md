# Project Structure

```mermaid
graph LR
    A[Project Root]
    A --- B[db]
    A --- C[models]
    A --- D[routers]
    A --- E[services]
    A --- F[utils]
    A --- G[config.py]
    A --- H[create_sessionurl_appmod.py]
    A --- I[main.py]
    A --- J[setup.py]
    A --- K[test.py]
    A --- L[requirements.txt]

    B --- B1[connection.py]
    B --- B2[firebase_init.py]

    C --- C1[cv_soln_models.py]
    C --- C2[cva_models.py]
    C --- C3[github_interaction_models.py]
    C --- C4[rlef_models.py]

    D --- D1[cv_solution]
    D --- D2[egpt_routes.py]
    D --- D3[git_interaction.py]
    D --- D4[rlef.py]
    D --- D5[user_management.py]

    D --> D1[cv_solution]
    D --> D2[egpt_routes.py]
    D --> D3[git_interaction.py]
    D --> D4[rlef.py]
    D --> D5[user_management.py]
