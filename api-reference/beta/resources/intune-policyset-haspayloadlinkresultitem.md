---
title: tipo de recurso hasPayloadLinkResultItem
description: Uma classe que contém o resultado da ação HasPayloadLinks.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 09e61f33151158c600e3a3ea783965f2f131fcce
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199648"
---
# <a name="haspayloadlinkresultitem-resource-type"></a><span data-ttu-id="81b40-103">tipo de recurso hasPayloadLinkResultItem</span><span class="sxs-lookup"><span data-stu-id="81b40-103">hasPayloadLinkResultItem resource type</span></span>

> <span data-ttu-id="81b40-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81b40-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81b40-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81b40-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81b40-106">Uma classe que contém o resultado da ação HasPayloadLinks.</span><span class="sxs-lookup"><span data-stu-id="81b40-106">A class containing the result of HasPayloadLinks action.</span></span>

## <a name="properties"></a><span data-ttu-id="81b40-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81b40-107">Properties</span></span>
|<span data-ttu-id="81b40-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81b40-108">Property</span></span>|<span data-ttu-id="81b40-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="81b40-109">Type</span></span>|<span data-ttu-id="81b40-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="81b40-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81b40-111">payloadId</span><span class="sxs-lookup"><span data-stu-id="81b40-111">payloadId</span></span>|<span data-ttu-id="81b40-112">String</span><span class="sxs-lookup"><span data-stu-id="81b40-112">String</span></span>|<span data-ttu-id="81b40-113">Chave da carga, no formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="81b40-113">Key of the Payload, In the format of Guid.</span></span>|
|<span data-ttu-id="81b40-114">hasLink</span><span class="sxs-lookup"><span data-stu-id="81b40-114">hasLink</span></span>|<span data-ttu-id="81b40-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="81b40-115">Boolean</span></span>|<span data-ttu-id="81b40-116">Indica se uma carga tem ou não um link.</span><span class="sxs-lookup"><span data-stu-id="81b40-116">Indicate whether a payload has any link or not.</span></span>|
|<span data-ttu-id="81b40-117">erro</span><span class="sxs-lookup"><span data-stu-id="81b40-117">error</span></span>|<span data-ttu-id="81b40-118">String</span><span class="sxs-lookup"><span data-stu-id="81b40-118">String</span></span>|<span data-ttu-id="81b40-119">Informação de exceção indica se a verificação desse item foi bem-sucedida ou não. Sequência vazia para nenhum erro.</span><span class="sxs-lookup"><span data-stu-id="81b40-119">Exception information indicates if check for this item was successful or not.Empty string for no error.</span></span>|
|<span data-ttu-id="81b40-120">fontes</span><span class="sxs-lookup"><span data-stu-id="81b40-120">sources</span></span>|<span data-ttu-id="81b40-121">coleção [deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md)</span><span class="sxs-lookup"><span data-stu-id="81b40-121">[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md) collection</span></span>|<span data-ttu-id="81b40-122">O motivo de origem do link.</span><span class="sxs-lookup"><span data-stu-id="81b40-122">The reason where the link comes from.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81b40-123">Relações</span><span class="sxs-lookup"><span data-stu-id="81b40-123">Relationships</span></span>
<span data-ttu-id="81b40-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81b40-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81b40-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81b40-125">JSON Representation</span></span>
<span data-ttu-id="81b40-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81b40-126">Here is a JSON representation of the resource.</span></span>
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



