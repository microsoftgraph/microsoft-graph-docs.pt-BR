---
title: Tipo de recurso deviceAppManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b99cd14d949d4043fe1ecb4b911c6f89a8f12b10
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756383"
---
# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="a0648-103">Tipo de recurso deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a0648-103">deviceAppManagement resource type</span></span>

<span data-ttu-id="a0648-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0648-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0648-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0648-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0648-106">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a0648-106">Singleton entity that acts as a container for all device app management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="a0648-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a0648-107">Methods</span></span>
|<span data-ttu-id="a0648-108">Método</span><span class="sxs-lookup"><span data-stu-id="a0648-108">Method</span></span>|<span data-ttu-id="a0648-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a0648-109">Return Type</span></span>|<span data-ttu-id="a0648-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0648-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a0648-111">Obter deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a0648-111">Get deviceAppManagement</span></span>](../api/intune-apps-deviceappmanagement-get.md)|[<span data-ttu-id="a0648-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a0648-112">deviceAppManagement</span></span>](../resources/intune-apps-deviceappmanagement.md)|<span data-ttu-id="a0648-113">Ler propriedades e relações de objetos de [deviceAppManagement](../resources/intune-apps-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="a0648-113">Read properties and relationships of the [deviceAppManagement](../resources/intune-apps-deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="a0648-114">Atualizar deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a0648-114">Update deviceAppManagement</span></span>](../api/intune-apps-deviceappmanagement-update.md)|[<span data-ttu-id="a0648-115">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a0648-115">deviceAppManagement</span></span>](../resources/intune-apps-deviceappmanagement.md)|<span data-ttu-id="a0648-116">Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune-apps-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="a0648-116">Update the properties of a [deviceAppManagement](../resources/intune-apps-deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a0648-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0648-117">Properties</span></span>
|<span data-ttu-id="a0648-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0648-118">Property</span></span>|<span data-ttu-id="a0648-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0648-119">Type</span></span>|<span data-ttu-id="a0648-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0648-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0648-121">id</span><span class="sxs-lookup"><span data-stu-id="a0648-121">id</span></span>|<span data-ttu-id="a0648-122">String</span><span class="sxs-lookup"><span data-stu-id="a0648-122">String</span></span>|<span data-ttu-id="a0648-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a0648-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0648-124">Relações</span><span class="sxs-lookup"><span data-stu-id="a0648-124">Relationships</span></span>
|<span data-ttu-id="a0648-125">Relação</span><span class="sxs-lookup"><span data-stu-id="a0648-125">Relationship</span></span>|<span data-ttu-id="a0648-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0648-126">Type</span></span>|<span data-ttu-id="a0648-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0648-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0648-128">mobileApps</span><span class="sxs-lookup"><span data-stu-id="a0648-128">mobileApps</span></span>|<span data-ttu-id="a0648-129">Coleção [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0648-129">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="a0648-130">Os aplicativos móveis.</span><span class="sxs-lookup"><span data-stu-id="a0648-130">The mobile apps.</span></span>|
|<span data-ttu-id="a0648-131">mobileAppCategories</span><span class="sxs-lookup"><span data-stu-id="a0648-131">mobileAppCategories</span></span>|<span data-ttu-id="a0648-132">Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="a0648-132">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="a0648-133">As categorias dos aplicativos móveis.</span><span class="sxs-lookup"><span data-stu-id="a0648-133">The mobile app categories.</span></span>|
|<span data-ttu-id="a0648-134">mobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="a0648-134">mobileAppConfigurations</span></span>|<span data-ttu-id="a0648-135">Coleção [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0648-135">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="a0648-136">As configurações de aplicativos móveis de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a0648-136">The Managed Device Mobile Application Configurations.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0648-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0648-137">JSON Representation</span></span>
<span data-ttu-id="a0648-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0648-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```




