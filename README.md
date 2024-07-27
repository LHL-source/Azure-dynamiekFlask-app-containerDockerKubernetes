
# Project: Azure-Dynamische Flask-App met Container, Docker en Kubernetes

## Doel van het Project
Het doel van dit project is om de implementatie van een dynamische Flask-webapplicatie te demonstreren met behulp van Docker-containers, Kubernetes-orkestratie en Azure-services, specifiek Azure Container Registry (ACR) en Azure Kubernetes Services (AKS). Deze setup zorgt voor schaalbaarheid, fouttolerantie en efficiënt resourcebeheer.

## Gedetailleerde Beschrijving
In dit project wordt een eenvoudige Flask-applicatie gecontaineriseerd met Docker en vervolgens geïmplementeerd in een Kubernetes-cluster beheerd door Azure Kubernetes Services (AKS). Het Docker-image wordt opgeslagen in de Azure Container Registry (ACR). Deze aanpak laat moderne applicatie-implementatiepraktijken zien, met de nadruk op containerisatie en orkestratie.

## Installatie-instructies
### Vereisten
1. **Flask Applicatie**: Een Python-webapplicatie gebouwd met Flask, inclusief afhankelijkheden gespecificeerd in `requirements.txt` en `runtime.txt`.
2. **Kubernetes-Implementatieconfiguratie**: Een `kubernetes-deployment.yaml` bestand voor het implementeren van de applicatie in het AKS-cluster.
3. **Benodigde Tools**:
   - Docker: Voor het bouwen en testen van container-images.
   - Kubectl: Kubernetes-commandoregeltool voor interactie met het cluster.
   - Azure CLI: Commandoregeltool voor het beheren van Azure-resources.

### Stappen
1. **Instellen van de Ontwikkelomgeving**:
   - Zorg ervoor dat de Flask-app (`app.py`) lokaal werkt.
   - Test de applicatie met de benodigde afhankelijkheden.

2. **Containerisatie**:
   - Maak een Dockerfile om de omgeving en afhankelijkheden te definiëren.
   - Bouw en test het Docker-image lokaal om ervoor te zorgen dat het correct functioneert.

3. **Azure Container Registry (ACR)**:
   - Maak een ACR aan om Docker-images te hosten.
   - Push het Docker-image naar de ACR.

4. **Azure Kubernetes Service (AKS)**:
   - Maak een AKS-cluster aan om de containers van de applicatie te beheren.
   - Configureer `kubectl` om verbinding te maken met het AKS-cluster.

5. **Implementatie**:
   - Gebruik Kubernetes-manifesten (YAML-bestanden) om de applicatie in het AKS-cluster te implementeren.
   - Stel de applicatie bloot via een externe service om toegang te krijgen via een browser.

## Overzicht van het Plan
1. **Project Setup en Voorbereiding**
   - Verifieer de Flask-applicatie lokaal.
   - Zorg voor toegang tot een Azure-account en stel de nodige permissies in.
   - Installeer Docker, kubectl en Azure CLI.

2. **Containerisatie met Docker**
   - Ontwikkel een Dockerfile voor de Flask-app.
   - Bouw het Docker-image en test het.

3. **Instellen van Azure Container Registry (ACR)**
   - Registreer een ACR-instantie en push het Docker-image naar de registry.

4. **Instellen van Azure Kubernetes Service (AKS)**
   - Implementeer een AKS-cluster.
   - Configureer kubectl voor het AKS-cluster.

5. **Implementatie van de Applicatie**
   - Implementeer de Flask-app met behulp van Kubernetes-deployment en serviceconfiguraties.
   - Test de implementatie en verifieer de beschikbaarheid van de applicatie.

---

