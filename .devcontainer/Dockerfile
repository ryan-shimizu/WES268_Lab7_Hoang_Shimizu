# Base image
FROM debian:bookworm-slim

# Install TeX Live and useful tools
RUN apt-get update && apt-get install -y \
    texlive-latex-recommended \
    texlive-latex-extra \
    texlive-fonts-recommended \
    texlive-fonts-extra \
    texlive-bibtex-extra \
    texlive-science \
    latexmk \
    biber \
    make \
    git \
    perl \
    && apt-get clean && rm -rf /var/lib/apt/lists/*

# Set working directory
WORKDIR /workspace