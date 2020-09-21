---
title: tipo de recurso hasPayloadLinkResultItem
description: Uma classe que contém o resultado da ação HasPayloadLinks.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 56c5631ed85f68942758b1283128f4f24ca53d45
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993501"
---
# <a name="haspayloadlinkresultitem-resource-type"></a><span data-ttu-id="e5df6-103">tipo de recurso hasPayloadLinkResultItem</span><span class="sxs-lookup"><span data-stu-id="e5df6-103">hasPayloadLinkResultItem resource type</span></span>

<span data-ttu-id="e5df6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5df6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5df6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e5df6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5df6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e5df6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5df6-107">Uma classe que contém o resultado da ação HasPayloadLinks.</span><span class="sxs-lookup"><span data-stu-id="e5df6-107">A class containing the result of HasPayloadLinks action.</span></span>

## <a name="properties"></a><span data-ttu-id="e5df6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5df6-108">Properties</span></span>
|<span data-ttu-id="e5df6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5df6-109">Property</span></span>|<span data-ttu-id="e5df6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5df6-110">Type</span></span>|<span data-ttu-id="e5df6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5df6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5df6-112">payloadId</span><span class="sxs-lookup"><span data-stu-id="e5df6-112">payloadId</span></span>|<span data-ttu-id="e5df6-113">String</span><span class="sxs-lookup"><span data-stu-id="e5df6-113">String</span></span>|<span data-ttu-id="e5df6-114">Chave da carga, no formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="e5df6-114">Key of the Payload, In the format of Guid.</span></span>|
|<span data-ttu-id="e5df6-115">hasLink</span><span class="sxs-lookup"><span data-stu-id="e5df6-115">hasLink</span></span>|<span data-ttu-id="e5df6-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5df6-116">Boolean</span></span>|<span data-ttu-id="e5df6-117">Indica se uma carga tem ou não um link.</span><span class="sxs-lookup"><span data-stu-id="e5df6-117">Indicate whether a payload has any link or not.</span></span>|
|<span data-ttu-id="e5df6-118">erro</span><span class="sxs-lookup"><span data-stu-id="e5df6-118">error</span></span>|<span data-ttu-id="e5df6-119">String</span><span class="sxs-lookup"><span data-stu-id="e5df6-119">String</span></span>|<span data-ttu-id="e5df6-120">Informação de exceção indica se a verificação desse item foi bem-sucedida ou não. Sequência vazia para nenhum erro.</span><span class="sxs-lookup"><span data-stu-id="e5df6-120">Exception information indicates if check for this item was successful or not.Empty string for no error.</span></span>|
|<span data-ttu-id="e5df6-121">fontes</span><span class="sxs-lookup"><span data-stu-id="e5df6-121">sources</span></span>|<span data-ttu-id="e5df6-122">coleção [deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md)</span><span class="sxs-lookup"><span data-stu-id="e5df6-122">[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md) collection</span></span>|<span data-ttu-id="e5df6-123">O motivo de origem do link.</span><span class="sxs-lookup"><span data-stu-id="e5df6-123">The reason where the link comes from.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5df6-124">Relações</span><span class="sxs-lookup"><span data-stu-id="e5df6-124">Relationships</span></span>
<span data-ttu-id="e5df6-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5df6-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5df6-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5df6-126">JSON Representation</span></span>
<span data-ttu-id="e5df6-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5df6-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hasPayloadLinkResultItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hasPayloadLinkResultItem",
  "payloadId": "String",
  "hasLink": true,
  "error": "String",
  "sources": [
    "String"
  ]
}
```






