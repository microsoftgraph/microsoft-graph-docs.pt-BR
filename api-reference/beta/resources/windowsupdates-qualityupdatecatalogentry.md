---
title: Tipo de recurso qualityUpdateCatalogEntry
description: Metadados para uma atualização Windows 10 de qualidade que você pode aprovar para implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: f455919bfc3d5f0e6c4e2aa5ef6a6b630b66bc52
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067791"
---
# <a name="qualityupdatecatalogentry-resource-type"></a><span data-ttu-id="4731e-103">Tipo de recurso qualityUpdateCatalogEntry</span><span class="sxs-lookup"><span data-stu-id="4731e-103">qualityUpdateCatalogEntry resource type</span></span>

<span data-ttu-id="4731e-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="4731e-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4731e-105">Metadados para uma atualização Windows 10 de qualidade que você pode aprovar para implantação.</span><span class="sxs-lookup"><span data-stu-id="4731e-105">Metadata for a Windows 10 quality update that you can be approve for deployment.</span></span>

<span data-ttu-id="4731e-106">Windows 10 de qualidade são lançadas uma ou mais vezes por mês.</span><span class="sxs-lookup"><span data-stu-id="4731e-106">Windows 10 quality updates are released one or more times per month.</span></span> <span data-ttu-id="4731e-107">Essas atualizações contêm correções de segurança e qualidade e geralmente são lançadas na segunda terça-feira de cada mês, embora possam ser lançadas a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="4731e-107">These updates contain both security and quality fixes and are typically released on the second Tuesday of every month, though they may be released at any time.</span></span> <span data-ttu-id="4731e-108">Essas atualizações são cumulativas, portanto, as versões posteriores sempre contêm todas as correções anteriores.</span><span class="sxs-lookup"><span data-stu-id="4731e-108">These updates are cumulative, so later versions always contain all previous fixes.</span></span> <span data-ttu-id="4731e-109">A Microsoft recomenda manter os dispositivos atualizados instalando as atualizações de qualidade mais recentes assim que elas estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="4731e-109">Microsoft strongly recommends keeping devices current by installing the most recent quality updates as soon as they are available.</span></span> 

<span data-ttu-id="4731e-110">Herda de [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="4731e-110">Inherits from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4731e-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4731e-111">Properties</span></span>
|<span data-ttu-id="4731e-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4731e-112">Property</span></span>|<span data-ttu-id="4731e-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="4731e-113">Type</span></span>|<span data-ttu-id="4731e-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="4731e-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4731e-115">deployableUntilDateTime</span><span class="sxs-lookup"><span data-stu-id="4731e-115">deployableUntilDateTime</span></span>|<span data-ttu-id="4731e-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4731e-116">DateTimeOffset</span></span>|<span data-ttu-id="4731e-117">A data em que o conteúdo não está mais disponível para implantação usando o serviço.</span><span class="sxs-lookup"><span data-stu-id="4731e-117">The date on which the content is no longer available for deployment using the service.</span></span> <span data-ttu-id="4731e-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4731e-118">Read-only.</span></span> <span data-ttu-id="4731e-119">Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="4731e-119">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="4731e-120">displayName</span><span class="sxs-lookup"><span data-stu-id="4731e-120">displayName</span></span>|<span data-ttu-id="4731e-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4731e-121">String</span></span>|<span data-ttu-id="4731e-122">O nome de exibição do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4731e-122">The display name of the content.</span></span> <span data-ttu-id="4731e-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4731e-123">Read-only.</span></span> <span data-ttu-id="4731e-124">Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="4731e-124">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="4731e-125">id</span><span class="sxs-lookup"><span data-stu-id="4731e-125">id</span></span>|<span data-ttu-id="4731e-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4731e-126">String</span></span>|<span data-ttu-id="4731e-127">O identificador exclusivo para a entrada do catálogo.</span><span class="sxs-lookup"><span data-stu-id="4731e-127">The unique identifier for the catalog entry.</span></span> <span data-ttu-id="4731e-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4731e-128">Read-only.</span></span> <span data-ttu-id="4731e-129">Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="4731e-129">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="4731e-130">isExpeditable</span><span class="sxs-lookup"><span data-stu-id="4731e-130">isExpeditable</span></span>|<span data-ttu-id="4731e-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="4731e-131">Boolean</span></span>|<span data-ttu-id="4731e-132">Indica se o conteúdo pode ser implantado como uma atualização de qualidade acelerada.</span><span class="sxs-lookup"><span data-stu-id="4731e-132">Indicates whether the content can be deployed as an expedited quality update.</span></span> <span data-ttu-id="4731e-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4731e-133">Read-only.</span></span>|
|<span data-ttu-id="4731e-134">qualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="4731e-134">qualityUpdateClassification</span></span>|<span data-ttu-id="4731e-135">microsoft.graph.windowsUpdates.qualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="4731e-135">microsoft.graph.windowsUpdates.qualityUpdateClassification</span></span>|<span data-ttu-id="4731e-136">A classificação na atualização de qualidade.</span><span class="sxs-lookup"><span data-stu-id="4731e-136">The classification on the quality update.</span></span> <span data-ttu-id="4731e-137">Oferece suporte a um subconjunto dos valores **para qualityUpdateClassification**.</span><span class="sxs-lookup"><span data-stu-id="4731e-137">Supports a subset of the values for **qualityUpdateClassification**.</span></span> <span data-ttu-id="4731e-138">Os valores possíveis são: `all`, `security`, `nonSecurity`.</span><span class="sxs-lookup"><span data-stu-id="4731e-138">Possible values are: `all`, `security`, `nonSecurity`.</span></span> <span data-ttu-id="4731e-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4731e-139">Read-only.</span></span>|
|<span data-ttu-id="4731e-140">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="4731e-140">releaseDateTime</span></span>|<span data-ttu-id="4731e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4731e-141">DateTimeOffset</span></span>|<span data-ttu-id="4731e-142">A data de lançamento do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4731e-142">The release date of the content.</span></span> <span data-ttu-id="4731e-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4731e-143">Read-only.</span></span> <span data-ttu-id="4731e-144">Herdado [de softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="4731e-144">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="4731e-145">Relações</span><span class="sxs-lookup"><span data-stu-id="4731e-145">Relationships</span></span>
<span data-ttu-id="4731e-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4731e-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4731e-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4731e-147">JSON representation</span></span>
<span data-ttu-id="4731e-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4731e-148">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
  "baseType": "microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)",
  "isExpeditable": "Boolean",
  "qualityUpdateClassification": "String"
}
```

