---
title: tipo de recurso hasPayloadLinkResultItem
description: Uma classe que contém o resultado da ação HasPayloadLinks.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4c6cc5e2f51265f062b6556438a177e4842e04e1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222475"
---
# <a name="haspayloadlinkresultitem-resource-type"></a><span data-ttu-id="b6b28-103">tipo de recurso hasPayloadLinkResultItem</span><span class="sxs-lookup"><span data-stu-id="b6b28-103">hasPayloadLinkResultItem resource type</span></span>

<span data-ttu-id="b6b28-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6b28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6b28-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b6b28-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6b28-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6b28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6b28-107">Uma classe que contém o resultado da ação HasPayloadLinks.</span><span class="sxs-lookup"><span data-stu-id="b6b28-107">A class containing the result of HasPayloadLinks action.</span></span>

## <a name="properties"></a><span data-ttu-id="b6b28-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6b28-108">Properties</span></span>
|<span data-ttu-id="b6b28-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6b28-109">Property</span></span>|<span data-ttu-id="b6b28-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6b28-110">Type</span></span>|<span data-ttu-id="b6b28-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6b28-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6b28-112">payloadId</span><span class="sxs-lookup"><span data-stu-id="b6b28-112">payloadId</span></span>|<span data-ttu-id="b6b28-113">String</span><span class="sxs-lookup"><span data-stu-id="b6b28-113">String</span></span>|<span data-ttu-id="b6b28-114">Chave da carga, no formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="b6b28-114">Key of the Payload, In the format of Guid.</span></span>|
|<span data-ttu-id="b6b28-115">hasLink</span><span class="sxs-lookup"><span data-stu-id="b6b28-115">hasLink</span></span>|<span data-ttu-id="b6b28-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6b28-116">Boolean</span></span>|<span data-ttu-id="b6b28-117">Indica se uma carga tem ou não um link.</span><span class="sxs-lookup"><span data-stu-id="b6b28-117">Indicate whether a payload has any link or not.</span></span>|
|<span data-ttu-id="b6b28-118">erro</span><span class="sxs-lookup"><span data-stu-id="b6b28-118">error</span></span>|<span data-ttu-id="b6b28-119">String</span><span class="sxs-lookup"><span data-stu-id="b6b28-119">String</span></span>|<span data-ttu-id="b6b28-120">Informação de exceção indica se a verificação desse item foi bem-sucedida ou não. Sequência vazia para nenhum erro.</span><span class="sxs-lookup"><span data-stu-id="b6b28-120">Exception information indicates if check for this item was successful or not.Empty string for no error.</span></span>|
|<span data-ttu-id="b6b28-121">fontes</span><span class="sxs-lookup"><span data-stu-id="b6b28-121">sources</span></span>|<span data-ttu-id="b6b28-122">coleção [deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md)</span><span class="sxs-lookup"><span data-stu-id="b6b28-122">[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md) collection</span></span>|<span data-ttu-id="b6b28-123">O motivo de origem do link.</span><span class="sxs-lookup"><span data-stu-id="b6b28-123">The reason where the link comes from.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6b28-124">Relações</span><span class="sxs-lookup"><span data-stu-id="b6b28-124">Relationships</span></span>
<span data-ttu-id="b6b28-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b6b28-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6b28-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6b28-126">JSON Representation</span></span>
<span data-ttu-id="b6b28-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6b28-127">Here is a JSON representation of the resource.</span></span>
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




