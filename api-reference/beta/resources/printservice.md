---
title: tipo de recurso de serviço de serviço
description: Representa uma descrição específica do locatário do Azure AD de uma instância de serviço de impressão. Existem serviços para cada componente da infraestrutura de impressão (por exemplo, descoberta, notificações, registro e IPP) e ter um ou mais pontos de extremidade.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 00ba50369f2396250df632c13ed3945e8c9d40d1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052535"
---
# <a name="printservice-resource-type"></a><span data-ttu-id="aca1f-104">tipo de recurso de serviço de serviço</span><span class="sxs-lookup"><span data-stu-id="aca1f-104">printService resource type</span></span>

<span data-ttu-id="aca1f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aca1f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aca1f-106">Representa uma descrição específica do locatário do Azure AD de uma instância de serviço de impressão.</span><span class="sxs-lookup"><span data-stu-id="aca1f-106">Represents an Azure AD tenant-specific description of a print service instance.</span></span> <span data-ttu-id="aca1f-107">Os serviços existem para cada componente da infraestrutura de impressão (descoberta, notificações, registro e IPP) e ter um ou mais pontos de extremidade.</span><span class="sxs-lookup"><span data-stu-id="aca1f-107">Services exist for each component of the printing infrastructure (discovery, notifications, registration, and IPP) and have one or more endpoints.</span></span>

## <a name="methods"></a><span data-ttu-id="aca1f-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="aca1f-108">Methods</span></span>

| <span data-ttu-id="aca1f-109">Método</span><span class="sxs-lookup"><span data-stu-id="aca1f-109">Method</span></span>       | <span data-ttu-id="aca1f-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="aca1f-110">Return Type</span></span> | <span data-ttu-id="aca1f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="aca1f-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="aca1f-112">Listar serviços</span><span class="sxs-lookup"><span data-stu-id="aca1f-112">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="aca1f-113">coleção de [serviços de multiserviço](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="aca1f-113">[printService](printservice.md) collection</span></span> | <span data-ttu-id="aca1f-114">Obtenha uma lista de serviços de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="aca1f-114">Get a list of Universal Print services.</span></span> |
| [<span data-ttu-id="aca1f-115">Obter serviço</span><span class="sxs-lookup"><span data-stu-id="aca1f-115">Get service</span></span>](../api/printservice-get.md) | [<span data-ttu-id="aca1f-116">Serviço de serviço</span><span class="sxs-lookup"><span data-stu-id="aca1f-116">printService</span></span>](printservice.md) | <span data-ttu-id="aca1f-117">Leia as propriedades e as relações do objeto de serviço.</span><span class="sxs-lookup"><span data-stu-id="aca1f-117">Read the properties and relationships of service object.</span></span> |
| [<span data-ttu-id="aca1f-118">Listar pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="aca1f-118">List endpoints</span></span>](../api/printservice-list-endpoints.md) | <span data-ttu-id="aca1f-119">coleção [Barserviceendpoint](printserviceendpoint.md)</span><span class="sxs-lookup"><span data-stu-id="aca1f-119">[printServiceEndpoint](printserviceendpoint.md) collection</span></span> | <span data-ttu-id="aca1f-120">Obter uma lista de pontos de extremidade que um serviço fornece.</span><span class="sxs-lookup"><span data-stu-id="aca1f-120">Get a list of endpoints that a service provides.</span></span> |

## <a name="properties"></a><span data-ttu-id="aca1f-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aca1f-121">Properties</span></span>
| <span data-ttu-id="aca1f-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aca1f-122">Property</span></span>     | <span data-ttu-id="aca1f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="aca1f-123">Type</span></span>        | <span data-ttu-id="aca1f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="aca1f-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="aca1f-125">id</span><span class="sxs-lookup"><span data-stu-id="aca1f-125">id</span></span>|<span data-ttu-id="aca1f-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aca1f-126">String</span></span>|<span data-ttu-id="aca1f-127">O identificador do serviço.</span><span class="sxs-lookup"><span data-stu-id="aca1f-127">The service's identifier.</span></span> <span data-ttu-id="aca1f-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aca1f-128">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aca1f-129">Relações</span><span class="sxs-lookup"><span data-stu-id="aca1f-129">Relationships</span></span>
| <span data-ttu-id="aca1f-130">Relação</span><span class="sxs-lookup"><span data-stu-id="aca1f-130">Relationship</span></span> | <span data-ttu-id="aca1f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="aca1f-131">Type</span></span>        | <span data-ttu-id="aca1f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="aca1f-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="aca1f-133">pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="aca1f-133">endpoints</span></span>|<span data-ttu-id="aca1f-134">coleção [Barserviceendpoint](printserviceendpoint.md)</span><span class="sxs-lookup"><span data-stu-id="aca1f-134">[printServiceEndpoint](printserviceendpoint.md) collection</span></span>| <span data-ttu-id="aca1f-135">Pontos de extremidade que podem ser usados para acessar o serviço.</span><span class="sxs-lookup"><span data-stu-id="aca1f-135">Endpoints that can be used to access the service.</span></span> <span data-ttu-id="aca1f-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aca1f-136">Read-only.</span></span> <span data-ttu-id="aca1f-137">Anulável.</span><span class="sxs-lookup"><span data-stu-id="aca1f-137">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aca1f-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aca1f-138">JSON representation</span></span>

<span data-ttu-id="aca1f-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aca1f-139">The following is a JSON representation of the resource.</span></span>

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

