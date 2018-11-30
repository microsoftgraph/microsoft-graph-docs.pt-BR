---
title: tipo de recurso de conector
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 6d4cb7e5ca1a5384dbb6c8be92e7ce4eb107388a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039596"
---
# <a name="connector-resource-type"></a><span data-ttu-id="a5cb7-103">tipo de recurso de conector</span><span class="sxs-lookup"><span data-stu-id="a5cb7-103">connector resource type</span></span>

> <span data-ttu-id="a5cb7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5cb7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-105">Use of these APIs in production applications is not supported.</span></span>

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="a5cb7-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="a5cb7-106">Methods</span></span>

| <span data-ttu-id="a5cb7-107">Método</span><span class="sxs-lookup"><span data-stu-id="a5cb7-107">Method</span></span>           | <span data-ttu-id="a5cb7-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a5cb7-108">Return Type</span></span>    |<span data-ttu-id="a5cb7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5cb7-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a5cb7-110">Obtenha o conector</span><span class="sxs-lookup"><span data-stu-id="a5cb7-110">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="a5cb7-111">conector</span><span class="sxs-lookup"><span data-stu-id="a5cb7-111">connector</span></span>](connector.md) |<span data-ttu-id="a5cb7-112">Leia as propriedades e os relacionamentos de objeto de conector.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-112">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="a5cb7-113">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="a5cb7-113">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="a5cb7-114">coleção [connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="a5cb7-114">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="a5cb7-115">Obtenha o objeto de connectorGroup associado com o conector.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-115">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="a5cb7-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a5cb7-116">Properties</span></span>
| <span data-ttu-id="a5cb7-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5cb7-117">Property</span></span>     | <span data-ttu-id="a5cb7-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5cb7-118">Type</span></span>   |<span data-ttu-id="a5cb7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5cb7-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5cb7-120">externalIp</span><span class="sxs-lookup"><span data-stu-id="a5cb7-120">externalIp</span></span>|<span data-ttu-id="a5cb7-121">String</span><span class="sxs-lookup"><span data-stu-id="a5cb7-121">String</span></span>|<span data-ttu-id="a5cb7-122">O endereço IP externo como detectada pelo serviço para a máquina do conector.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-122">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="a5cb7-123">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="a5cb7-123">Read-only</span></span>|
|<span data-ttu-id="a5cb7-124">id</span><span class="sxs-lookup"><span data-stu-id="a5cb7-124">id</span></span>|<span data-ttu-id="a5cb7-125">String</span><span class="sxs-lookup"><span data-stu-id="a5cb7-125">String</span></span>| <span data-ttu-id="a5cb7-126">A id de objeto do conector.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-126">The object id of the connector.</span></span> <BR><span data-ttu-id="a5cb7-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-127">Read-only.</span></span>|
|<span data-ttu-id="a5cb7-128">machineName</span><span class="sxs-lookup"><span data-stu-id="a5cb7-128">machineName</span></span>|<span data-ttu-id="a5cb7-129">String</span><span class="sxs-lookup"><span data-stu-id="a5cb7-129">String</span></span>| <span data-ttu-id="a5cb7-130">O nome do computador que está executando o conector.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-130">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="a5cb7-131">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="a5cb7-131">Read-only</span></span>|
|<span data-ttu-id="a5cb7-132">status</span><span class="sxs-lookup"><span data-stu-id="a5cb7-132">status</span></span>|<span data-ttu-id="a5cb7-133">string</span><span class="sxs-lookup"><span data-stu-id="a5cb7-133">string</span></span>| <span data-ttu-id="a5cb7-134">Indica o status do conector.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-134">Indicates the status of the connector.</span></span> <span data-ttu-id="a5cb7-135">Os valores possíveis são: `active` e `inactive`.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-135">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="a5cb7-136">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="a5cb7-136">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="a5cb7-137">Relações</span><span class="sxs-lookup"><span data-stu-id="a5cb7-137">Relationships</span></span>
| <span data-ttu-id="a5cb7-138">Relação</span><span class="sxs-lookup"><span data-stu-id="a5cb7-138">Relationship</span></span> | <span data-ttu-id="a5cb7-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5cb7-139">Type</span></span>   |<span data-ttu-id="a5cb7-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5cb7-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5cb7-141">memberOf</span><span class="sxs-lookup"><span data-stu-id="a5cb7-141">memberOf</span></span>|<span data-ttu-id="a5cb7-142">coleção [connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="a5cb7-142">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="a5cb7-143">O connectorGroup conectar é membro de.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-143">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="a5cb7-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-144">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a5cb7-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a5cb7-145">JSON representation</span></span>

<span data-ttu-id="a5cb7-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-146">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
