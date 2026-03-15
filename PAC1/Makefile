ENVNAME = uoc2026pec1
PYTHONVER = 3.13

install:
	@echo "Installing dependencies..."
	conda create -n $(ENVNAME) python=$(PYTHONVER) -y
	conda activate $(ENVNAME) && pip install -r requirements.txt