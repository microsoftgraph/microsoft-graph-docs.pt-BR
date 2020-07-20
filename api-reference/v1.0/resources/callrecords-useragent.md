---
title: tipo de recurso UserAgent
description: O tipo UserAgent
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 795332d58359d0a0a5dd2776f6c93923fe1bafd8
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491939"
---
# <a name="useragent-resource-type"></a><span data-ttu-id="0bbf3-103">tipo de recurso UserAgent</span><span class="sxs-lookup"><span data-stu-id="0bbf3-103">userAgent resource type</span></span>

<span data-ttu-id="0bbf3-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="0bbf3-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="0bbf3-105">Representa o agente do usuário de um ponto de extremidade em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="0bbf3-105">Represents the user agent of an endpoint in a call.</span></span>
<span data-ttu-id="0bbf3-106">Os tipos [clientUserAgent](callrecords-clientuseragent.md) e [serviceUserAgent](callrecords-serviceuseragent.md)) são herdados desse tipo.</span><span class="sxs-lookup"><span data-stu-id="0bbf3-106">The [clientUserAgent](callrecords-clientuseragent.md) and [serviceUserAgent](callrecords-serviceuseragent.md)) types inherit from this type.</span></span>

## <a name="properties"></a><span data-ttu-id="0bbf3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0bbf3-107">Properties</span></span>

| <span data-ttu-id="0bbf3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bbf3-108">Property</span></span>     | <span data-ttu-id="0bbf3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bbf3-109">Type</span></span>        | <span data-ttu-id="0bbf3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bbf3-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0bbf3-111">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="0bbf3-111">applicationVersion</span></span>|<span data-ttu-id="0bbf3-112">String</span><span class="sxs-lookup"><span data-stu-id="0bbf3-112">String</span></span>|<span data-ttu-id="0bbf3-113">Identifica a versão do software do aplicativo usado por esse ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="0bbf3-113">Identifies the version of application software used by this endpoint.</span></span>|
|<span data-ttu-id="0bbf3-114">headerValue</span><span class="sxs-lookup"><span data-stu-id="0bbf3-114">headerValue</span></span>|<span data-ttu-id="0bbf3-115">String</span><span class="sxs-lookup"><span data-stu-id="0bbf3-115">String</span></span>|<span data-ttu-id="0bbf3-116">Valor do cabeçalho do agente de usuário relatado por esse ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="0bbf3-116">User-agent header value reported by this endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0bbf3-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0bbf3-117">JSON representation</span></span>

<span data-ttu-id="0bbf3-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0bbf3-118">The following is a JSON representation of the resource.</span></span>

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