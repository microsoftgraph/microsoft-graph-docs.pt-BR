---
title: tipo de recurso de fileserviceendpoint
description: Representa as informações de identificação e URI de uma instância de serviço de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 8b9289807778c1a44940d8e8eb0d9163ed12f006
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985857"
---
# <a name="printserviceendpoint-resource-type"></a><span data-ttu-id="10d24-103">tipo de recurso de fileserviceendpoint</span><span class="sxs-lookup"><span data-stu-id="10d24-103">printServiceEndpoint resource type</span></span>

<span data-ttu-id="10d24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10d24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10d24-105">Representa as informações de identificação e URI de uma instância de serviço de impressão.</span><span class="sxs-lookup"><span data-stu-id="10d24-105">Represents URI and identifying information for a print service instance.</span></span>

## <a name="methods"></a><span data-ttu-id="10d24-106">Methods</span><span class="sxs-lookup"><span data-stu-id="10d24-106">Methods</span></span>

| <span data-ttu-id="10d24-107">Método</span><span class="sxs-lookup"><span data-stu-id="10d24-107">Method</span></span>       | <span data-ttu-id="10d24-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="10d24-108">Return Type</span></span> | <span data-ttu-id="10d24-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="10d24-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="10d24-110">Obter o ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="10d24-110">Get endpoint</span></span>](../api/printserviceendpoint-get.md) | [<span data-ttu-id="10d24-111">fileserviceendpoint</span><span class="sxs-lookup"><span data-stu-id="10d24-111">printServiceEndpoint</span></span>](printserviceendpoint.md) | <span data-ttu-id="10d24-112">Leia as propriedades e os relacionamentos do objeto de ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="10d24-112">Read the properties and relationships of endpoint object.</span></span> |

## <a name="properties"></a><span data-ttu-id="10d24-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10d24-113">Properties</span></span>
| <span data-ttu-id="10d24-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10d24-114">Property</span></span>     | <span data-ttu-id="10d24-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="10d24-115">Type</span></span>        | <span data-ttu-id="10d24-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="10d24-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="10d24-117">displayName</span><span class="sxs-lookup"><span data-stu-id="10d24-117">displayName</span></span>|<span data-ttu-id="10d24-118">String</span><span class="sxs-lookup"><span data-stu-id="10d24-118">String</span></span>|<span data-ttu-id="10d24-119">Um nome de exibição legível para o ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="10d24-119">A human-readable display name for the endpoint.</span></span>|
|<span data-ttu-id="10d24-120">nome</span><span class="sxs-lookup"><span data-stu-id="10d24-120">name</span></span>|<span data-ttu-id="10d24-121">String</span><span class="sxs-lookup"><span data-stu-id="10d24-121">String</span></span>|<span data-ttu-id="10d24-122">Um nome exclusivo que identifica o serviço que o ponto de extremidade fornece.</span><span class="sxs-lookup"><span data-stu-id="10d24-122">A unique name that identifies the service that the endpoint provides.</span></span> <span data-ttu-id="10d24-123">Os valores possíveis são: `discovery` (serviço de descoberta), `notification` (serviço de notificação), `ipp` (serviço IPP) e `registration` (serviço de registro).</span><span class="sxs-lookup"><span data-stu-id="10d24-123">Possible values are: `discovery` (Discovery Service), `notification` (Notification Service), `ipp` (IPP Service), and `registration` (Registration Service).</span></span> <span data-ttu-id="10d24-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="10d24-124">Read-only.</span></span>|
|<span data-ttu-id="10d24-125">URI</span><span class="sxs-lookup"><span data-stu-id="10d24-125">uri</span></span>|<span data-ttu-id="10d24-126">String</span><span class="sxs-lookup"><span data-stu-id="10d24-126">String</span></span>|<span data-ttu-id="10d24-127">O URI que pode ser usado para acessar o serviço.</span><span class="sxs-lookup"><span data-stu-id="10d24-127">The URI that can be used to access the service.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10d24-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10d24-128">JSON representation</span></span>

<span data-ttu-id="10d24-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10d24-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printServiceEndpoint"
}-->

```json
{
  "displayName": "String",
  "name": "String (identifier)",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printServiceEndpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

