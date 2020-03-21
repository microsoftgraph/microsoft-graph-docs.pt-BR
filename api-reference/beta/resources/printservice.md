---
title: tipo de recurso de serviço de serviço
description: Representa uma descrição específica do locatário do Azure AD de uma instância de serviço de impressão. Existem serviços para cada componente da infraestrutura de impressão (por exemplo, descoberta, notificações, registro e IPP) e ter um ou mais pontos de extremidade.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: fd8641f7fe9fd361e131f0978c8f677a6395e405
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895500"
---
# <a name="printservice-resource-type"></a><span data-ttu-id="1026e-104">tipo de recurso de serviço de serviço</span><span class="sxs-lookup"><span data-stu-id="1026e-104">printService resource type</span></span>

<span data-ttu-id="1026e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1026e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1026e-106">Representa uma descrição específica do locatário do Azure AD de uma instância de serviço de impressão.</span><span class="sxs-lookup"><span data-stu-id="1026e-106">Represents an Azure AD tenant-specific description of a print service instance.</span></span> <span data-ttu-id="1026e-107">Os serviços existem para cada componente da infraestrutura de impressão (descoberta, notificações, registro e IPP) e ter um ou mais pontos de extremidade.</span><span class="sxs-lookup"><span data-stu-id="1026e-107">Services exist for each component of the printing infrastructure (discovery, notifications, registration, and IPP) and have one or more endpoints.</span></span>

## <a name="methods"></a><span data-ttu-id="1026e-108">Methods</span><span class="sxs-lookup"><span data-stu-id="1026e-108">Methods</span></span>

| <span data-ttu-id="1026e-109">Método</span><span class="sxs-lookup"><span data-stu-id="1026e-109">Method</span></span>       | <span data-ttu-id="1026e-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1026e-110">Return Type</span></span> | <span data-ttu-id="1026e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1026e-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1026e-112">Listar serviços</span><span class="sxs-lookup"><span data-stu-id="1026e-112">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="1026e-113">coleção de [serviços de multiserviço](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="1026e-113">[printService](printservice.md) collection</span></span> | <span data-ttu-id="1026e-114">Obtenha uma lista de serviços de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="1026e-114">Get a list of Universal Print services.</span></span> |
| [<span data-ttu-id="1026e-115">Obter serviço</span><span class="sxs-lookup"><span data-stu-id="1026e-115">Get service</span></span>](../api/printservice-get.md) | [<span data-ttu-id="1026e-116">Serviço de serviço</span><span class="sxs-lookup"><span data-stu-id="1026e-116">printService</span></span>](printservice.md) | <span data-ttu-id="1026e-117">Leia as propriedades e as relações do objeto de serviço.</span><span class="sxs-lookup"><span data-stu-id="1026e-117">Read the properties and relationships of service object.</span></span> |
| [<span data-ttu-id="1026e-118">Listar pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="1026e-118">List endpoints</span></span>](../api/printservice-list-endpoints.md) | <span data-ttu-id="1026e-119">coleção [Barserviceendpoint](printserviceendpoint.md)</span><span class="sxs-lookup"><span data-stu-id="1026e-119">[printServiceEndpoint](printserviceendpoint.md) collection</span></span> | <span data-ttu-id="1026e-120">Obter uma lista de pontos de extremidade que um serviço fornece.</span><span class="sxs-lookup"><span data-stu-id="1026e-120">Get a list of endpoints that a service provides.</span></span> |

## <a name="properties"></a><span data-ttu-id="1026e-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1026e-121">Properties</span></span>
| <span data-ttu-id="1026e-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1026e-122">Property</span></span>     | <span data-ttu-id="1026e-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="1026e-123">Type</span></span>        | <span data-ttu-id="1026e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1026e-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1026e-125">id</span><span class="sxs-lookup"><span data-stu-id="1026e-125">id</span></span>|<span data-ttu-id="1026e-126">String</span><span class="sxs-lookup"><span data-stu-id="1026e-126">String</span></span>|<span data-ttu-id="1026e-127">O identificador do serviço.</span><span class="sxs-lookup"><span data-stu-id="1026e-127">The service's identifier.</span></span> <span data-ttu-id="1026e-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1026e-128">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1026e-129">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="1026e-129">Relationships</span></span>
| <span data-ttu-id="1026e-130">Relação</span><span class="sxs-lookup"><span data-stu-id="1026e-130">Relationship</span></span> | <span data-ttu-id="1026e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1026e-131">Type</span></span>        | <span data-ttu-id="1026e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1026e-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1026e-133">pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="1026e-133">endpoints</span></span>|<span data-ttu-id="1026e-134">coleção [Barserviceendpoint](printserviceendpoint.md)</span><span class="sxs-lookup"><span data-stu-id="1026e-134">[printServiceEndpoint](printserviceendpoint.md) collection</span></span>| <span data-ttu-id="1026e-135">Pontos de extremidade que podem ser usados para acessar o serviço.</span><span class="sxs-lookup"><span data-stu-id="1026e-135">Endpoints that can be used to access the service.</span></span> <span data-ttu-id="1026e-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1026e-136">Read-only.</span></span> <span data-ttu-id="1026e-137">Anulável.</span><span class="sxs-lookup"><span data-stu-id="1026e-137">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1026e-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1026e-138">JSON representation</span></span>

<span data-ttu-id="1026e-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1026e-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printService",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "endpoints": [ {"@odata.type": "microsoft.graph.printServiceEndpoint"} ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->