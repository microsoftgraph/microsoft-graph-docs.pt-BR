---
title: tipo de recurso cloudPcStatusDetails
description: Os detalhes do status do PC de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 647c13878e054fbac6c1f43f565bd2788d19a9de
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378265"
---
# <a name="cloudpcstatusdetails-resource-type"></a><span data-ttu-id="846b6-103">tipo de recurso cloudPcStatusDetails</span><span class="sxs-lookup"><span data-stu-id="846b6-103">cloudPcStatusDetails resource type</span></span>

<span data-ttu-id="846b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="846b6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="846b6-105">Os detalhes do status do PC de nuvem.</span><span class="sxs-lookup"><span data-stu-id="846b6-105">The details of the cloud PC status.</span></span>

## <a name="properties"></a><span data-ttu-id="846b6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="846b6-106">Properties</span></span>

|<span data-ttu-id="846b6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="846b6-107">Property</span></span>|<span data-ttu-id="846b6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="846b6-108">Type</span></span>|<span data-ttu-id="846b6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="846b6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="846b6-110">código</span><span class="sxs-lookup"><span data-stu-id="846b6-110">code</span></span>|<span data-ttu-id="846b6-111">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="846b6-111">String</span></span>|<span data-ttu-id="846b6-112">O código associado ao status do PC de nuvem.</span><span class="sxs-lookup"><span data-stu-id="846b6-112">The code associated with the cloud PC status.</span></span>|
|<span data-ttu-id="846b6-113">mensagem</span><span class="sxs-lookup"><span data-stu-id="846b6-113">message</span></span>|<span data-ttu-id="846b6-114">String</span><span class="sxs-lookup"><span data-stu-id="846b6-114">String</span></span>|<span data-ttu-id="846b6-115">A mensagem de status.</span><span class="sxs-lookup"><span data-stu-id="846b6-115">The status message.</span></span>|
|<span data-ttu-id="846b6-116">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="846b6-116">additionalInformation</span></span>|<span data-ttu-id="846b6-117">Coleção [KeyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="846b6-117">[KeyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="846b6-118">Informações adicionais sobre o status do PC de nuvem.</span><span class="sxs-lookup"><span data-stu-id="846b6-118">Any additional information about the cloud PC status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="846b6-119">Relações</span><span class="sxs-lookup"><span data-stu-id="846b6-119">Relationships</span></span>

<span data-ttu-id="846b6-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="846b6-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="846b6-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="846b6-121">JSON representation</span></span>

<span data-ttu-id="846b6-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="846b6-122">The following is a JSON representation of the resource.</span></span>
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
