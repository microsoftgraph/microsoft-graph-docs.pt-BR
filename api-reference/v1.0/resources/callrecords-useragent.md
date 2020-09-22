---
title: tipo de recurso UserAgent
description: O tipo UserAgent
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 54acb771330bf77e3361450bd032193e0cf65466
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069306"
---
# <a name="useragent-resource-type"></a><span data-ttu-id="dd8e5-103">tipo de recurso UserAgent</span><span class="sxs-lookup"><span data-stu-id="dd8e5-103">userAgent resource type</span></span>

<span data-ttu-id="dd8e5-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="dd8e5-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="dd8e5-105">Representa o agente do usuário de um ponto de extremidade em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="dd8e5-105">Represents the user agent of an endpoint in a call.</span></span>
<span data-ttu-id="dd8e5-106">Os tipos [clientUserAgent](callrecords-clientuseragent.md) e [serviceUserAgent](callrecords-serviceuseragent.md)) são herdados desse tipo.</span><span class="sxs-lookup"><span data-stu-id="dd8e5-106">The [clientUserAgent](callrecords-clientuseragent.md) and [serviceUserAgent](callrecords-serviceuseragent.md)) types inherit from this type.</span></span>

## <a name="properties"></a><span data-ttu-id="dd8e5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd8e5-107">Properties</span></span>

| <span data-ttu-id="dd8e5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd8e5-108">Property</span></span>     | <span data-ttu-id="dd8e5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd8e5-109">Type</span></span>        | <span data-ttu-id="dd8e5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd8e5-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dd8e5-111">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="dd8e5-111">applicationVersion</span></span>|<span data-ttu-id="dd8e5-112">String</span><span class="sxs-lookup"><span data-stu-id="dd8e5-112">String</span></span>|<span data-ttu-id="dd8e5-113">Identifica a versão do software do aplicativo usado por esse ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="dd8e5-113">Identifies the version of application software used by this endpoint.</span></span>|
|<span data-ttu-id="dd8e5-114">headerValue</span><span class="sxs-lookup"><span data-stu-id="dd8e5-114">headerValue</span></span>|<span data-ttu-id="dd8e5-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd8e5-115">String</span></span>|<span data-ttu-id="dd8e5-116">Valor do cabeçalho do agente de usuário relatado por esse ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="dd8e5-116">User-agent header value reported by this endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dd8e5-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd8e5-117">JSON representation</span></span>

<span data-ttu-id="dd8e5-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dd8e5-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.userAgent",
  "baseType": null
}-->

```json
{
  "applicationVersion": "String",
  "headerValue": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
