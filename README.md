# Instalar o requirements.txt

pip install -r requirements.txt


# Inicializar o alembic

python -m alembic init migrations


python -m alembic revision --autogenerate -m "Criar tabela usuario"


python -m alembic upgrade head


python -m uvicorn app.main:app --reload