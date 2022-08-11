# Base image to use for demos.

# Tag will be automatically generated through pre-commit hook if any changes
# happened in the docker/ folder
FROM projectnessie/nessie-binder-demos:d7ef1150a637df2bf805a8e3d224a2d6a503829d

# Create the necessary folders for the demo, this will be created and owned by {NB_USER}
RUN mkdir -p notebooks && mkdir -p datasets

# Copy the python notebooks into the existing notebooks folder
COPY notebooks/*.ipynb notebooks/

# Copy all the needed datasets for the demos
COPY datasets/ datasets/
