---
title: tipo de recurso cloudPcStatusDetails
description: Os detalhes do status do PC de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 61260bc7f3437fe1f10575afc616462eec2e47dc
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563828"
---
# <a name="cloudpcstatusdetails-resource-type"></a><span data-ttu-id="ee8f3-103">tipo de recurso cloudPcStatusDetails</span><span class="sxs-lookup"><span data-stu-id="ee8f3-103">cloudPcStatusDetails resource type</span></span>

<span data-ttu-id="ee8f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee8f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee8f3-105">Os detalhes do status do PC de nuvem.</span><span class="sxs-lookup"><span data-stu-id="ee8f3-105">The details of the cloud PC status.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="ee8f3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee8f3-106">Properties</span></span>

|<span data-ttu-id="ee8f3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee8f3-107">Property</span></span>|<span data-ttu-id="ee8f3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee8f3-108">Type</span></span>|<span data-ttu-id="ee8f3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee8f3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee8f3-110">código</span><span class="sxs-lookup"><span data-stu-id="ee8f3-110">code</span></span>|<span data-ttu-id="ee8f3-111">String</span><span class="sxs-lookup"><span data-stu-id="ee8f3-111">String</span></span>|<span data-ttu-id="ee8f3-112">O código associado ao status do PC de nuvem.</span><span class="sxs-lookup"><span data-stu-id="ee8f3-112">The code associated with the cloud PC status.</span></span>|
|<span data-ttu-id="ee8f3-113">mensagem</span><span class="sxs-lookup"><span data-stu-id="ee8f3-113">message</span></span>|<span data-ttu-id="ee8f3-114">String</span><span class="sxs-lookup"><span data-stu-id="ee8f3-114">String</span></span>|<span data-ttu-id="ee8f3-115">A mensagem de status.</span><span class="sxs-lookup"><span data-stu-id="ee8f3-115">The status message.</span></span>|
|<span data-ttu-id="ee8f3-116">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="ee8f3-116">additionalInformation</span></span>|<span data-ttu-id="ee8f3-117">Coleção [KeyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ee8f3-117">[KeyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="ee8f3-118">Informações adicionais sobre o status do PC de nuvem.</span><span class="sxs-lookup"><span data-stu-id="ee8f3-118">Any additional information about the cloud PC status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee8f3-119">Relações</span><span class="sxs-lookup"><span data-stu-id="ee8f3-119">Relationships</span></span>

<span data-ttu-id="ee8f3-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee8f3-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee8f3-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee8f3-121">JSON representation</span></span>

<span data-ttu-id="ee8f3-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee8f3-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcStatusDetails",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcStatusDetails",
  "code": "String",
  "message": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```
