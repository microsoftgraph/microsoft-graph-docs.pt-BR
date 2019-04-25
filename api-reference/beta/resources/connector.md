---
title: tipo de recurso conector
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: eed936c808e920f35a741a836a1fab64b2754bf8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535519"
---
# <a name="connector-resource-type"></a><span data-ttu-id="6bd6a-103">tipo de recurso conector</span><span class="sxs-lookup"><span data-stu-id="6bd6a-103">connector resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="6bd6a-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="6bd6a-104">Methods</span></span>

| <span data-ttu-id="6bd6a-105">Método</span><span class="sxs-lookup"><span data-stu-id="6bd6a-105">Method</span></span>           | <span data-ttu-id="6bd6a-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6bd6a-106">Return Type</span></span>    |<span data-ttu-id="6bd6a-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bd6a-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6bd6a-108">Obter conector</span><span class="sxs-lookup"><span data-stu-id="6bd6a-108">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="6bd6a-109">conector</span><span class="sxs-lookup"><span data-stu-id="6bd6a-109">connector</span></span>](connector.md) |<span data-ttu-id="6bd6a-110">Leia as propriedades e as relações do objeto Connector.</span><span class="sxs-lookup"><span data-stu-id="6bd6a-110">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="6bd6a-111">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="6bd6a-111">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="6bd6a-112">[](connectorgroup.md) coleção de conectores</span><span class="sxs-lookup"><span data-stu-id="6bd6a-112">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="6bd6a-113">Obtenha o objeto de conexão associado ao conector.</span><span class="sxs-lookup"><span data-stu-id="6bd6a-113">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="6bd6a-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6bd6a-114">Properties</span></span>
| <span data-ttu-id="6bd6a-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6bd6a-115">Property</span></span>     | <span data-ttu-id="6bd6a-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bd6a-116">Type</span></span>   |<span data-ttu-id="6bd6a-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bd6a-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6bd6a-118">externalIp</span><span class="sxs-lookup"><span data-stu-id="6bd6a-118">externalIp</span></span>|<span data-ttu-id="6bd6a-119">String</span><span class="sxs-lookup"><span data-stu-id="6bd6a-119">String</span></span>|<span data-ttu-id="6bd6a-120">O endereço IP externo, conforme detectado pelo serviço para o computador do conector.</span><span class="sxs-lookup"><span data-stu-id="6bd6a-120">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="6bd6a-121">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="6bd6a-121">Read-only</span></span>|
|<span data-ttu-id="6bd6a-122">id</span><span class="sxs-lookup"><span data-stu-id="6bd6a-122">id</span></span>|<span data-ttu-id="6bd6a-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6bd6a-123">String</span></span>| <span data-ttu-id="6bd6a-124">A ID de objeto do conector.</span><span class="sxs-lookup"><span data-stu-id="6bd6a-124">The object id of the connector.</span></span> <BR><span data-ttu-id="6bd6a-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6bd6a-125">Read-only.</span></span>|
|<span data-ttu-id="6bd6a-126">Nomecomputador</span><span class="sxs-lookup"><span data-stu-id="6bd6a-126">machineName</span></span>|<span data-ttu-id="6bd6a-127">String</span><span class="sxs-lookup"><span data-stu-id="6bd6a-127">String</span></span>| <span data-ttu-id="6bd6a-128">O nome da máquina na qual o conector está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="6bd6a-128">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="6bd6a-129">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="6bd6a-129">Read-only</span></span>|
|<span data-ttu-id="6bd6a-130">status</span><span class="sxs-lookup"><span data-stu-id="6bd6a-130">status</span></span>|<span data-ttu-id="6bd6a-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6bd6a-131">string</span></span>| <span data-ttu-id="6bd6a-132">Indica o status do conector.</span><span class="sxs-lookup"><span data-stu-id="6bd6a-132">Indicates the status of the connector.</span></span> <span data-ttu-id="6bd6a-133">Os valores possíveis são: `active` e `inactive`.</span><span class="sxs-lookup"><span data-stu-id="6bd6a-133">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="6bd6a-134">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="6bd6a-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="6bd6a-135">Relações</span><span class="sxs-lookup"><span data-stu-id="6bd6a-135">Relationships</span></span>
| <span data-ttu-id="6bd6a-136">Relação</span><span class="sxs-lookup"><span data-stu-id="6bd6a-136">Relationship</span></span> | <span data-ttu-id="6bd6a-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bd6a-137">Type</span></span>   |<span data-ttu-id="6bd6a-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bd6a-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6bd6a-139">memberOf</span><span class="sxs-lookup"><span data-stu-id="6bd6a-139">memberOf</span></span>|<span data-ttu-id="6bd6a-140">[](connectorgroup.md) coleção de conectores</span><span class="sxs-lookup"><span data-stu-id="6bd6a-140">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="6bd6a-141">O MemberGroup do qual a conexão é membro.</span><span class="sxs-lookup"><span data-stu-id="6bd6a-141">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="6bd6a-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6bd6a-142">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6bd6a-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6bd6a-143">JSON representation</span></span>

<span data-ttu-id="6bd6a-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6bd6a-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/connector.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
