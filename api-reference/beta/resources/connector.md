---
title: tipo de recurso conector
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 5467d2a4625ad3813ff2777838db87be3ca5b713
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341208"
---
# <a name="connector-resource-type"></a><span data-ttu-id="65172-103">tipo de recurso conector</span><span class="sxs-lookup"><span data-stu-id="65172-103">connector resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="65172-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="65172-104">Methods</span></span>

| <span data-ttu-id="65172-105">Método</span><span class="sxs-lookup"><span data-stu-id="65172-105">Method</span></span>           | <span data-ttu-id="65172-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="65172-106">Return Type</span></span>    |<span data-ttu-id="65172-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="65172-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="65172-108">Obter conector</span><span class="sxs-lookup"><span data-stu-id="65172-108">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="65172-109">conector</span><span class="sxs-lookup"><span data-stu-id="65172-109">connector</span></span>](connector.md) |<span data-ttu-id="65172-110">Leia as propriedades e as relações do objeto Connector.</span><span class="sxs-lookup"><span data-stu-id="65172-110">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="65172-111">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="65172-111">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="65172-112">[](connectorgroup.md) coleção de conectores</span><span class="sxs-lookup"><span data-stu-id="65172-112">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="65172-113">Obtenha o objeto de conexão associado ao conector.</span><span class="sxs-lookup"><span data-stu-id="65172-113">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="65172-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65172-114">Properties</span></span>
| <span data-ttu-id="65172-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65172-115">Property</span></span>     | <span data-ttu-id="65172-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="65172-116">Type</span></span>   |<span data-ttu-id="65172-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="65172-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65172-118">externalIp</span><span class="sxs-lookup"><span data-stu-id="65172-118">externalIp</span></span>|<span data-ttu-id="65172-119">String</span><span class="sxs-lookup"><span data-stu-id="65172-119">String</span></span>|<span data-ttu-id="65172-120">O endereço IP externo, conforme detectado pelo serviço para o computador do conector.</span><span class="sxs-lookup"><span data-stu-id="65172-120">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="65172-121">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="65172-121">Read-only</span></span>|
|<span data-ttu-id="65172-122">id</span><span class="sxs-lookup"><span data-stu-id="65172-122">id</span></span>|<span data-ttu-id="65172-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65172-123">String</span></span>| <span data-ttu-id="65172-124">A ID de objeto do conector.</span><span class="sxs-lookup"><span data-stu-id="65172-124">The object id of the connector.</span></span> <BR><span data-ttu-id="65172-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="65172-125">Read-only.</span></span>|
|<span data-ttu-id="65172-126">Nomecomputador</span><span class="sxs-lookup"><span data-stu-id="65172-126">machineName</span></span>|<span data-ttu-id="65172-127">String</span><span class="sxs-lookup"><span data-stu-id="65172-127">String</span></span>| <span data-ttu-id="65172-128">O nome da máquina na qual o conector está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="65172-128">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="65172-129">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="65172-129">Read-only</span></span>|
|<span data-ttu-id="65172-130">status</span><span class="sxs-lookup"><span data-stu-id="65172-130">status</span></span>|<span data-ttu-id="65172-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65172-131">string</span></span>| <span data-ttu-id="65172-132">Indica o status do conector.</span><span class="sxs-lookup"><span data-stu-id="65172-132">Indicates the status of the connector.</span></span> <span data-ttu-id="65172-133">Os valores possíveis são: `active` e `inactive`.</span><span class="sxs-lookup"><span data-stu-id="65172-133">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="65172-134">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="65172-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="65172-135">Relações</span><span class="sxs-lookup"><span data-stu-id="65172-135">Relationships</span></span>
| <span data-ttu-id="65172-136">Relação</span><span class="sxs-lookup"><span data-stu-id="65172-136">Relationship</span></span> | <span data-ttu-id="65172-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="65172-137">Type</span></span>   |<span data-ttu-id="65172-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="65172-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65172-139">memberOf</span><span class="sxs-lookup"><span data-stu-id="65172-139">memberOf</span></span>|<span data-ttu-id="65172-140">[](connectorgroup.md) coleção de conectores</span><span class="sxs-lookup"><span data-stu-id="65172-140">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="65172-141">O MemberGroup do qual a conexão é membro.</span><span class="sxs-lookup"><span data-stu-id="65172-141">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="65172-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="65172-142">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="65172-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65172-143">JSON representation</span></span>

<span data-ttu-id="65172-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65172-144">Here is a JSON representation of the resource.</span></span>

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
