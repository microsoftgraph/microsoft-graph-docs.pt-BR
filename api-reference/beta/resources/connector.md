---
title: tipo de recurso conector
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 25d350e48aaddbda2b931ae5a9e177ec6caa9799
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507475"
---
# <a name="connector-resource-type"></a><span data-ttu-id="02a53-103">tipo de recurso conector</span><span class="sxs-lookup"><span data-stu-id="02a53-103">connector resource type</span></span>

<span data-ttu-id="02a53-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="02a53-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="02a53-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="02a53-105">Methods</span></span>

| <span data-ttu-id="02a53-106">Método</span><span class="sxs-lookup"><span data-stu-id="02a53-106">Method</span></span>           | <span data-ttu-id="02a53-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="02a53-107">Return Type</span></span>    |<span data-ttu-id="02a53-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="02a53-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="02a53-109">Obter conector</span><span class="sxs-lookup"><span data-stu-id="02a53-109">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="02a53-110">conector</span><span class="sxs-lookup"><span data-stu-id="02a53-110">connector</span></span>](connector.md) |<span data-ttu-id="02a53-111">Leia as propriedades e as relações do objeto Connector.</span><span class="sxs-lookup"><span data-stu-id="02a53-111">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="02a53-112">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="02a53-112">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="02a53-113">coleção de [conectores](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="02a53-113">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="02a53-114">Obtenha o objeto de conexão associado ao conector.</span><span class="sxs-lookup"><span data-stu-id="02a53-114">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="02a53-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="02a53-115">Properties</span></span>
| <span data-ttu-id="02a53-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02a53-116">Property</span></span>     | <span data-ttu-id="02a53-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="02a53-117">Type</span></span>   |<span data-ttu-id="02a53-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="02a53-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02a53-119">externalIp</span><span class="sxs-lookup"><span data-stu-id="02a53-119">externalIp</span></span>|<span data-ttu-id="02a53-120">String</span><span class="sxs-lookup"><span data-stu-id="02a53-120">String</span></span>|<span data-ttu-id="02a53-121">O endereço IP externo, conforme detectado pelo serviço para o computador do conector.</span><span class="sxs-lookup"><span data-stu-id="02a53-121">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="02a53-122">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="02a53-122">Read-only</span></span>|
|<span data-ttu-id="02a53-123">id</span><span class="sxs-lookup"><span data-stu-id="02a53-123">id</span></span>|<span data-ttu-id="02a53-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02a53-124">String</span></span>| <span data-ttu-id="02a53-125">A ID de objeto do conector.</span><span class="sxs-lookup"><span data-stu-id="02a53-125">The object id of the connector.</span></span> <BR><span data-ttu-id="02a53-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="02a53-126">Read-only.</span></span>|
|<span data-ttu-id="02a53-127">Nomecomputador</span><span class="sxs-lookup"><span data-stu-id="02a53-127">machineName</span></span>|<span data-ttu-id="02a53-128">String</span><span class="sxs-lookup"><span data-stu-id="02a53-128">String</span></span>| <span data-ttu-id="02a53-129">O nome da máquina na qual o conector está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="02a53-129">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="02a53-130">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="02a53-130">Read-only</span></span>|
|<span data-ttu-id="02a53-131">status</span><span class="sxs-lookup"><span data-stu-id="02a53-131">status</span></span>|<span data-ttu-id="02a53-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02a53-132">string</span></span>| <span data-ttu-id="02a53-133">Indica o status do conector.</span><span class="sxs-lookup"><span data-stu-id="02a53-133">Indicates the status of the connector.</span></span> <span data-ttu-id="02a53-134">Os valores possíveis são: `active` e `inactive`.</span><span class="sxs-lookup"><span data-stu-id="02a53-134">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="02a53-135">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="02a53-135">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="02a53-136">Relações</span><span class="sxs-lookup"><span data-stu-id="02a53-136">Relationships</span></span>
| <span data-ttu-id="02a53-137">Relação</span><span class="sxs-lookup"><span data-stu-id="02a53-137">Relationship</span></span> | <span data-ttu-id="02a53-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="02a53-138">Type</span></span>   |<span data-ttu-id="02a53-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="02a53-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02a53-140">memberOf</span><span class="sxs-lookup"><span data-stu-id="02a53-140">memberOf</span></span>|<span data-ttu-id="02a53-141">coleção de [conectores](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="02a53-141">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="02a53-142">O MemberGroup do qual a conexão é membro.</span><span class="sxs-lookup"><span data-stu-id="02a53-142">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="02a53-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="02a53-143">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="02a53-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="02a53-144">JSON representation</span></span>

<span data-ttu-id="02a53-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="02a53-145">Here is a JSON representation of the resource.</span></span>

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
