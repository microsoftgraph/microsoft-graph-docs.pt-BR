---
title: tipo de recurso conector
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ec4d3fdb415533d5b3f2effc72688fe912551bc8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012874"
---
# <a name="connector-resource-type"></a><span data-ttu-id="49b75-103">tipo de recurso conector</span><span class="sxs-lookup"><span data-stu-id="49b75-103">connector resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="49b75-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="49b75-104">Methods</span></span>

| <span data-ttu-id="49b75-105">Método</span><span class="sxs-lookup"><span data-stu-id="49b75-105">Method</span></span>           | <span data-ttu-id="49b75-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="49b75-106">Return Type</span></span>    |<span data-ttu-id="49b75-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="49b75-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="49b75-108">Obter conector</span><span class="sxs-lookup"><span data-stu-id="49b75-108">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="49b75-109">conector</span><span class="sxs-lookup"><span data-stu-id="49b75-109">connector</span></span>](connector.md) |<span data-ttu-id="49b75-110">Leia as propriedades e as relações do objeto Connector.</span><span class="sxs-lookup"><span data-stu-id="49b75-110">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="49b75-111">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="49b75-111">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="49b75-112">[](connectorgroup.md) coleção de conectores</span><span class="sxs-lookup"><span data-stu-id="49b75-112">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="49b75-113">Obtenha o objeto de conexão associado ao conector.</span><span class="sxs-lookup"><span data-stu-id="49b75-113">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="49b75-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="49b75-114">Properties</span></span>
| <span data-ttu-id="49b75-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49b75-115">Property</span></span>     | <span data-ttu-id="49b75-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="49b75-116">Type</span></span>   |<span data-ttu-id="49b75-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="49b75-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49b75-118">externalIp</span><span class="sxs-lookup"><span data-stu-id="49b75-118">externalIp</span></span>|<span data-ttu-id="49b75-119">String</span><span class="sxs-lookup"><span data-stu-id="49b75-119">String</span></span>|<span data-ttu-id="49b75-120">O endereço IP externo, conforme detectado pelo serviço para o computador do conector.</span><span class="sxs-lookup"><span data-stu-id="49b75-120">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="49b75-121">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="49b75-121">Read-only</span></span>|
|<span data-ttu-id="49b75-122">id</span><span class="sxs-lookup"><span data-stu-id="49b75-122">id</span></span>|<span data-ttu-id="49b75-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49b75-123">String</span></span>| <span data-ttu-id="49b75-124">A ID de objeto do conector.</span><span class="sxs-lookup"><span data-stu-id="49b75-124">The object id of the connector.</span></span> <BR><span data-ttu-id="49b75-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="49b75-125">Read-only.</span></span>|
|<span data-ttu-id="49b75-126">Nomecomputador</span><span class="sxs-lookup"><span data-stu-id="49b75-126">machineName</span></span>|<span data-ttu-id="49b75-127">String</span><span class="sxs-lookup"><span data-stu-id="49b75-127">String</span></span>| <span data-ttu-id="49b75-128">O nome da máquina na qual o conector está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="49b75-128">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="49b75-129">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="49b75-129">Read-only</span></span>|
|<span data-ttu-id="49b75-130">status</span><span class="sxs-lookup"><span data-stu-id="49b75-130">status</span></span>|<span data-ttu-id="49b75-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49b75-131">string</span></span>| <span data-ttu-id="49b75-132">Indica o status do conector.</span><span class="sxs-lookup"><span data-stu-id="49b75-132">Indicates the status of the connector.</span></span> <span data-ttu-id="49b75-133">Os valores possíveis são: `active` e `inactive`.</span><span class="sxs-lookup"><span data-stu-id="49b75-133">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="49b75-134">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="49b75-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="49b75-135">Relações</span><span class="sxs-lookup"><span data-stu-id="49b75-135">Relationships</span></span>
| <span data-ttu-id="49b75-136">Relação</span><span class="sxs-lookup"><span data-stu-id="49b75-136">Relationship</span></span> | <span data-ttu-id="49b75-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="49b75-137">Type</span></span>   |<span data-ttu-id="49b75-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="49b75-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49b75-139">memberOf</span><span class="sxs-lookup"><span data-stu-id="49b75-139">memberOf</span></span>|<span data-ttu-id="49b75-140">[](connectorgroup.md) coleção de conectores</span><span class="sxs-lookup"><span data-stu-id="49b75-140">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="49b75-141">O MemberGroup do qual a conexão é membro.</span><span class="sxs-lookup"><span data-stu-id="49b75-141">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="49b75-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="49b75-142">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="49b75-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="49b75-143">JSON representation</span></span>

<span data-ttu-id="49b75-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="49b75-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connector"
}-->

```json
{
  "externalIp": "String",
  "id": "String (identifier)",
  "machineName": "String",
  "status": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
