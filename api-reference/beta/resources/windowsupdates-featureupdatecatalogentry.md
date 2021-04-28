---
title: tipo de recurso featureUpdateCatalogEntry
description: Metadados para uma atualização Windows 10 de recursos que você pode aprovar para implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 64ad4c2506a2d8f90276e50e7fe5288e1af1d8db
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067251"
---
# <a name="featureupdatecatalogentry-resource-type"></a><span data-ttu-id="ff690-103">tipo de recurso featureUpdateCatalogEntry</span><span class="sxs-lookup"><span data-stu-id="ff690-103">featureUpdateCatalogEntry resource type</span></span>

<span data-ttu-id="ff690-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="ff690-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff690-105">Metadados para uma atualização Windows 10 de recursos que você pode aprovar para implantação.</span><span class="sxs-lookup"><span data-stu-id="ff690-105">Metadata for a Windows 10 feature update that you can approve for deployment.</span></span>

<span data-ttu-id="ff690-106">Windows 10 de recursos são lançadas anualmente e contêm novos recursos para Windows 10.</span><span class="sxs-lookup"><span data-stu-id="ff690-106">Windows 10 feature updates are released bi-annually and contain new features for Windows 10.</span></span> <span data-ttu-id="ff690-107">Instalar essas atualizações aumenta o número Windows 10 de com build e normalmente resulta em um novo ciclo de vida de manutenção e data de término do serviço.</span><span class="sxs-lookup"><span data-stu-id="ff690-107">Installing these updates increases the Windows 10 build number and typically results in a new servicing lifecycle and end of service date.</span></span> <span data-ttu-id="ff690-108">A Microsoft recomenda que as organizações implantem regularmente novas atualizações de recursos como parte da adoção Windows como um serviço.</span><span class="sxs-lookup"><span data-stu-id="ff690-108">Microsoft recommends organizations regularly deploy new feature updates as part of adopting Windows as a service.</span></span>

<span data-ttu-id="ff690-109">Herda de [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="ff690-109">Inherits from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ff690-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff690-110">Properties</span></span>
|<span data-ttu-id="ff690-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff690-111">Property</span></span>|<span data-ttu-id="ff690-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff690-112">Type</span></span>|<span data-ttu-id="ff690-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff690-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff690-114">deployableUntilDateTime</span><span class="sxs-lookup"><span data-stu-id="ff690-114">deployableUntilDateTime</span></span>|<span data-ttu-id="ff690-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff690-115">DateTimeOffset</span></span>|<span data-ttu-id="ff690-116">A data em que o conteúdo não está mais disponível para implantação usando o serviço.</span><span class="sxs-lookup"><span data-stu-id="ff690-116">The date on which the content is no longer available for deployment using the service.</span></span> <span data-ttu-id="ff690-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff690-117">Read-only.</span></span> <span data-ttu-id="ff690-118">Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="ff690-118">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="ff690-119">displayName</span><span class="sxs-lookup"><span data-stu-id="ff690-119">displayName</span></span>|<span data-ttu-id="ff690-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff690-120">String</span></span>|<span data-ttu-id="ff690-121">O nome de exibição do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ff690-121">The display name of the content.</span></span> <span data-ttu-id="ff690-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff690-122">Read-only.</span></span> <span data-ttu-id="ff690-123">Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="ff690-123">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="ff690-124">id</span><span class="sxs-lookup"><span data-stu-id="ff690-124">id</span></span>|<span data-ttu-id="ff690-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff690-125">String</span></span>|<span data-ttu-id="ff690-126">O identificador exclusivo para a entrada do catálogo.</span><span class="sxs-lookup"><span data-stu-id="ff690-126">The unique identifier for the catalog entry.</span></span> <span data-ttu-id="ff690-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff690-127">Read-only.</span></span> <span data-ttu-id="ff690-128">Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="ff690-128">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="ff690-129">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="ff690-129">releaseDateTime</span></span>|<span data-ttu-id="ff690-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff690-130">DateTimeOffset</span></span>|<span data-ttu-id="ff690-131">A data de lançamento do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ff690-131">The release date for the content.</span></span> <span data-ttu-id="ff690-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff690-132">Read-only.</span></span> <span data-ttu-id="ff690-133">Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="ff690-133">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="ff690-134">versão</span><span class="sxs-lookup"><span data-stu-id="ff690-134">version</span></span>|<span data-ttu-id="ff690-135">String</span><span class="sxs-lookup"><span data-stu-id="ff690-135">String</span></span>|<span data-ttu-id="ff690-136">A versão da atualização de recursos.</span><span class="sxs-lookup"><span data-stu-id="ff690-136">The version of the feature update.</span></span> <span data-ttu-id="ff690-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff690-137">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff690-138">Relações</span><span class="sxs-lookup"><span data-stu-id="ff690-138">Relationships</span></span>
<span data-ttu-id="ff690-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff690-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff690-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff690-140">JSON representation</span></span>
<span data-ttu-id="ff690-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff690-141">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
  "baseType": "microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)",
  "version": "String"
}
```

