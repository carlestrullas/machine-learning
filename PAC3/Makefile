ENVNAME = uoc2026pec3
PYTHONVER = 3.12

install:
	@echo "Installing dependencies..."
	conda create -n $(ENVNAME) python=$(PYTHONVER) -y
	conda activate $(ENVNAME) && pip install -r requirements.txt
