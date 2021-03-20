---
title: tipo de recurso do conector
description: Representa um conector proxy de aplicativo.
author: japere
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 567b67576c5300419c9671de8bd82df84bf49685
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945694"
---
# <a name="connector-resource-type"></a><span data-ttu-id="dc3f7-103">tipo de recurso do conector</span><span class="sxs-lookup"><span data-stu-id="dc3f7-103">connector resource type</span></span>

<span data-ttu-id="dc3f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc3f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc3f7-105">Os conectores são agentes leves que se sentam no local e facilitam a conexão de saída para o serviço proxy de aplicativo do [Azure AD.](https://aka.ms/whyappproxy)</span><span class="sxs-lookup"><span data-stu-id="dc3f7-105">Connectors are lightweight agents that sit on-premises and facilitate the outbound connection to the [Azure AD Application Proxy](https://aka.ms/whyappproxy) service.</span></span> <span data-ttu-id="dc3f7-106">Cada conector faz parte de um [connectorGroup](connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="dc3f7-106">Each connector is part of a [connectorGroup](connectorgroup.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dc3f7-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="dc3f7-107">Methods</span></span>

| <span data-ttu-id="dc3f7-108">Método</span><span class="sxs-lookup"><span data-stu-id="dc3f7-108">Method</span></span>       | <span data-ttu-id="dc3f7-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dc3f7-109">Return Type</span></span> | <span data-ttu-id="dc3f7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc3f7-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="dc3f7-111">Listar conectores</span><span class="sxs-lookup"><span data-stu-id="dc3f7-111">List connectors</span></span>](../api/connector-list.md) | <span data-ttu-id="dc3f7-112">[coleção connector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="dc3f7-112">[connector](connector.md) collection</span></span> | <span data-ttu-id="dc3f7-113">Recupere uma lista de objetos do conector.</span><span class="sxs-lookup"><span data-stu-id="dc3f7-113">Retrieve a list of connector objects.</span></span> | 
| [<span data-ttu-id="dc3f7-114">Obter conector</span><span class="sxs-lookup"><span data-stu-id="dc3f7-114">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="dc3f7-115">connector</span><span class="sxs-lookup"><span data-stu-id="dc3f7-115">connector</span></span>](connector.md) | <span data-ttu-id="dc3f7-116">Ler propriedades e relações do objeto connector.</span><span class="sxs-lookup"><span data-stu-id="dc3f7-116">Read properties and relationships of connector object.</span></span> |
| [<span data-ttu-id="dc3f7-117">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="dc3f7-117">List memberOf</span></span>](../api/connector-list-memberof.md) | <span data-ttu-id="dc3f7-118">[Coleção connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="dc3f7-118">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="dc3f7-119">Listar a coleção de objetos connectorGroup da que o conector é membro.</span><span class="sxs-lookup"><span data-stu-id="dc3f7-119">List the connectorGroup object collection the connector is a member of.</span></span> |
| [<span data-ttu-id="dc3f7-120">Adicionar conector a connectorGroup</span><span class="sxs-lookup"><span data-stu-id="dc3f7-120">Add connector to connectorGroup</span></span>](../api/connector-post-memberof.md)| [<span data-ttu-id="dc3f7-121">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="dc3f7-121">connectorGroup</span></span>](connectorgroup.md) | <span data-ttu-id="dc3f7-122">Adicione um conector a um connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="dc3f7-122">Add a connector to a connectorGroup.</span></span> |


## <a name="properties"></a><span data-ttu-id="dc3f7-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc3f7-123">Properties</span></span>
| <span data-ttu-id="dc3f7-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc3f7-124">Property</span></span>     | <span data-ttu-id="dc3f7-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc3f7-125">Type</span></span>        | <span data-ttu-id="dc3f7-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc3f7-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dc3f7-127">externalIp</span><span class="sxs-lookup"><span data-stu-id="dc3f7-127">externalIp</span></span>|<span data-ttu-id="dc3f7-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc3f7-128">String</span></span>| <span data-ttu-id="dc3f7-129">O endereço IP externo detectado pelo servidor do conector.</span><span class="sxs-lookup"><span data-stu-id="dc3f7-129">The external IP address as detected by the the connector server.</span></span> <span data-ttu-id="dc3f7-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dc3f7-130">Read-only.</span></span> |
|<span data-ttu-id="dc3f7-131">id</span><span class="sxs-lookup"><span data-stu-id="dc3f7-131">id</span></span>|<span data-ttu-id="dc3f7-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc3f7-132">String</span></span>| <span data-ttu-id="dc3f7-133">Identificador exclusivo do conector.</span><span class="sxs-lookup"><span data-stu-id="dc3f7-133">Unique identifier of the connector.</span></span> <span data-ttu-id="dc3f7-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dc3f7-134">Read-only.</span></span> |
|<span data-ttu-id="dc3f7-135">machineName</span><span class="sxs-lookup"><span data-stu-id="dc3f7-135">machineName</span></span>|<span data-ttu-id="dc3f7-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc3f7-136">String</span></span>| <span data-ttu-id="dc3f7-137">O nome do computador em que o conector está instalado e em execução.</span><span class="sxs-lookup"><span data-stu-id="dc3f7-137">The machine name the connector is installed and running on.</span></span> |
|<span data-ttu-id="dc3f7-138">status</span><span class="sxs-lookup"><span data-stu-id="dc3f7-138">status</span></span>|<span data-ttu-id="dc3f7-139">connectorStatus</span><span class="sxs-lookup"><span data-stu-id="dc3f7-139">connectorStatus</span></span>| <span data-ttu-id="dc3f7-140">Indica o status do conector.</span><span class="sxs-lookup"><span data-stu-id="dc3f7-140">Indicates the status of the connector.</span></span> <span data-ttu-id="dc3f7-141">Os valores possíveis são: `active` e `inactive`.</span><span class="sxs-lookup"><span data-stu-id="dc3f7-141">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="dc3f7-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dc3f7-142">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="dc3f7-143">Relações</span><span class="sxs-lookup"><span data-stu-id="dc3f7-143">Relationships</span></span>
| <span data-ttu-id="dc3f7-144">Relação</span><span class="sxs-lookup"><span data-stu-id="dc3f7-144">Relationship</span></span> | <span data-ttu-id="dc3f7-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc3f7-145">Type</span></span>   |<span data-ttu-id="dc3f7-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc3f7-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc3f7-147">memberOf</span><span class="sxs-lookup"><span data-stu-id="dc3f7-147">memberOf</span></span>|<span data-ttu-id="dc3f7-148">[Coleção connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="dc3f7-148">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="dc3f7-149">O connectorGroup do que o conector é membro.</span><span class="sxs-lookup"><span data-stu-id="dc3f7-149">The connectorGroup that the connector is a member of.</span></span> <span data-ttu-id="dc3f7-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dc3f7-150">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dc3f7-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc3f7-151">JSON representation</span></span>

<span data-ttu-id="dc3f7-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dc3f7-152">The following is a JSON representation of the resource.</span></span>

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



