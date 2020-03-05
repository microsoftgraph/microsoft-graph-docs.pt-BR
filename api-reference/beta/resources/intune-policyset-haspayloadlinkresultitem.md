---
title: tipo de recurso hasPayloadLinkResultItem
description: Uma classe que contém o resultado da ação HasPayloadLinks.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 219bf9b1a2058b06895ec90883849cc8bdf0b569
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524003"
---
# <a name="haspayloadlinkresultitem-resource-type"></a><span data-ttu-id="60e3f-103">tipo de recurso hasPayloadLinkResultItem</span><span class="sxs-lookup"><span data-stu-id="60e3f-103">hasPayloadLinkResultItem resource type</span></span>

<span data-ttu-id="60e3f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="60e3f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60e3f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="60e3f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60e3f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="60e3f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60e3f-107">Uma classe que contém o resultado da ação HasPayloadLinks.</span><span class="sxs-lookup"><span data-stu-id="60e3f-107">A class containing the result of HasPayloadLinks action.</span></span>

## <a name="properties"></a><span data-ttu-id="60e3f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60e3f-108">Properties</span></span>
|<span data-ttu-id="60e3f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60e3f-109">Property</span></span>|<span data-ttu-id="60e3f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="60e3f-110">Type</span></span>|<span data-ttu-id="60e3f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="60e3f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60e3f-112">payloadId</span><span class="sxs-lookup"><span data-stu-id="60e3f-112">payloadId</span></span>|<span data-ttu-id="60e3f-113">String</span><span class="sxs-lookup"><span data-stu-id="60e3f-113">String</span></span>|<span data-ttu-id="60e3f-114">Chave da carga, no formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="60e3f-114">Key of the Payload, In the format of Guid.</span></span>|
|<span data-ttu-id="60e3f-115">hasLink</span><span class="sxs-lookup"><span data-stu-id="60e3f-115">hasLink</span></span>|<span data-ttu-id="60e3f-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="60e3f-116">Boolean</span></span>|<span data-ttu-id="60e3f-117">Indica se uma carga tem ou não um link.</span><span class="sxs-lookup"><span data-stu-id="60e3f-117">Indicate whether a payload has any link or not.</span></span>|
|<span data-ttu-id="60e3f-118">erro</span><span class="sxs-lookup"><span data-stu-id="60e3f-118">error</span></span>|<span data-ttu-id="60e3f-119">String</span><span class="sxs-lookup"><span data-stu-id="60e3f-119">String</span></span>|<span data-ttu-id="60e3f-120">Informação de exceção indica se a verificação desse item foi bem-sucedida ou não. Sequência vazia para nenhum erro.</span><span class="sxs-lookup"><span data-stu-id="60e3f-120">Exception information indicates if check for this item was successful or not.Empty string for no error.</span></span>|
|<span data-ttu-id="60e3f-121">fontes</span><span class="sxs-lookup"><span data-stu-id="60e3f-121">sources</span></span>|<span data-ttu-id="60e3f-122">coleção [deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md)</span><span class="sxs-lookup"><span data-stu-id="60e3f-122">[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md) collection</span></span>|<span data-ttu-id="60e3f-123">O motivo de origem do link.</span><span class="sxs-lookup"><span data-stu-id="60e3f-123">The reason where the link comes from.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60e3f-124">Relações</span><span class="sxs-lookup"><span data-stu-id="60e3f-124">Relationships</span></span>
<span data-ttu-id="60e3f-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="60e3f-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60e3f-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60e3f-126">JSON Representation</span></span>
<span data-ttu-id="60e3f-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="60e3f-127">Here is a JSON representation of the resource.</span></span>
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



