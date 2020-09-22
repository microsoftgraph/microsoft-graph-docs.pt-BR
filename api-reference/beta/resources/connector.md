---
title: tipo de recurso conector
description: Representa um conector de proxy de aplicativo.
author: japere
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3e42bc42c1989e530f7b7f307da3963407ded112
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027164"
---
# <a name="connector-resource-type"></a><span data-ttu-id="ff31b-103">tipo de recurso conector</span><span class="sxs-lookup"><span data-stu-id="ff31b-103">connector resource type</span></span>

<span data-ttu-id="ff31b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff31b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff31b-105">Os conectores são agentes leves que ficam no local e facilitam a conexão de saída para o serviço de [proxy de aplicativo do Azure ad](https://aka.ms/whyappproxy) .</span><span class="sxs-lookup"><span data-stu-id="ff31b-105">Connectors are lightweight agents that sit on-premises and facilitate the outbound connection to the [Azure AD Application Proxy](https://aka.ms/whyappproxy) service.</span></span> <span data-ttu-id="ff31b-106">Cada conector é parte de um [conector](connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="ff31b-106">Each connector is part of a [connectorGroup](connectorgroup.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ff31b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ff31b-107">Methods</span></span>

| <span data-ttu-id="ff31b-108">Método</span><span class="sxs-lookup"><span data-stu-id="ff31b-108">Method</span></span>       | <span data-ttu-id="ff31b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ff31b-109">Return Type</span></span> | <span data-ttu-id="ff31b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff31b-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ff31b-111">Listar conectores</span><span class="sxs-lookup"><span data-stu-id="ff31b-111">List connectors</span></span>](../api/connector-list.md) | <span data-ttu-id="ff31b-112">coleção [Connector](connector.md)</span><span class="sxs-lookup"><span data-stu-id="ff31b-112">[connector](connector.md) collection</span></span> | <span data-ttu-id="ff31b-113">Recupere uma lista de objetos Connector.</span><span class="sxs-lookup"><span data-stu-id="ff31b-113">Retrieve a list of connector objects.</span></span> | 
| [<span data-ttu-id="ff31b-114">Obter conector</span><span class="sxs-lookup"><span data-stu-id="ff31b-114">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="ff31b-115">conector</span><span class="sxs-lookup"><span data-stu-id="ff31b-115">connector</span></span>](connector.md) | <span data-ttu-id="ff31b-116">Leia as propriedades e as relações do objeto Connector.</span><span class="sxs-lookup"><span data-stu-id="ff31b-116">Read properties and relationships of connector object.</span></span> |
| [<span data-ttu-id="ff31b-117">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="ff31b-117">List memberOf</span></span>](../api/connector-list-memberof.md) | <span data-ttu-id="ff31b-118">coleção de [conectores](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="ff31b-118">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="ff31b-119">Lista o conjunto de objetos do grupo de conectores do qual o conector é membro.</span><span class="sxs-lookup"><span data-stu-id="ff31b-119">List the connectorGroup object collection the connector is a member of.</span></span> |
| [<span data-ttu-id="ff31b-120">Adicionar conector a connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ff31b-120">Add connector to connectorGroup</span></span>](../api/connector-post-memberof.md)| [<span data-ttu-id="ff31b-121">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ff31b-121">connectorGroup</span></span>](connectorgroup.md) | <span data-ttu-id="ff31b-122">Adicionar um conector a um conector.</span><span class="sxs-lookup"><span data-stu-id="ff31b-122">Add a connector to a connectorGroup.</span></span> |


## <a name="properties"></a><span data-ttu-id="ff31b-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff31b-123">Properties</span></span>
| <span data-ttu-id="ff31b-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff31b-124">Property</span></span>     | <span data-ttu-id="ff31b-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff31b-125">Type</span></span>        | <span data-ttu-id="ff31b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff31b-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ff31b-127">externalIp</span><span class="sxs-lookup"><span data-stu-id="ff31b-127">externalIp</span></span>|<span data-ttu-id="ff31b-128">String</span><span class="sxs-lookup"><span data-stu-id="ff31b-128">String</span></span>| <span data-ttu-id="ff31b-129">O endereço IP externo, conforme detectado pelo servidor do conector.</span><span class="sxs-lookup"><span data-stu-id="ff31b-129">The external IP address as detected by the the connector server.</span></span> <span data-ttu-id="ff31b-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff31b-130">Read-only.</span></span> |
|<span data-ttu-id="ff31b-131">id</span><span class="sxs-lookup"><span data-stu-id="ff31b-131">id</span></span>|<span data-ttu-id="ff31b-132">String</span><span class="sxs-lookup"><span data-stu-id="ff31b-132">String</span></span>| <span data-ttu-id="ff31b-133">Identificador exclusivo do conector.</span><span class="sxs-lookup"><span data-stu-id="ff31b-133">Unique identifier of the connector.</span></span> <span data-ttu-id="ff31b-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff31b-134">Read-only.</span></span> |
|<span data-ttu-id="ff31b-135">Nomecomputador</span><span class="sxs-lookup"><span data-stu-id="ff31b-135">machineName</span></span>|<span data-ttu-id="ff31b-136">String</span><span class="sxs-lookup"><span data-stu-id="ff31b-136">String</span></span>| <span data-ttu-id="ff31b-137">O nome do computador no qual o conector está instalado e em execução.</span><span class="sxs-lookup"><span data-stu-id="ff31b-137">The machine name the connector is installed and running on.</span></span> |
|<span data-ttu-id="ff31b-138">status</span><span class="sxs-lookup"><span data-stu-id="ff31b-138">status</span></span>|<span data-ttu-id="ff31b-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff31b-139">string</span></span>| <span data-ttu-id="ff31b-140">Indica o status do conector.</span><span class="sxs-lookup"><span data-stu-id="ff31b-140">Indicates the status of the connector.</span></span> <span data-ttu-id="ff31b-141">Os valores possíveis são: `active` e `inactive`.</span><span class="sxs-lookup"><span data-stu-id="ff31b-141">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="ff31b-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff31b-142">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ff31b-143">Relações</span><span class="sxs-lookup"><span data-stu-id="ff31b-143">Relationships</span></span>
| <span data-ttu-id="ff31b-144">Relação</span><span class="sxs-lookup"><span data-stu-id="ff31b-144">Relationship</span></span> | <span data-ttu-id="ff31b-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff31b-145">Type</span></span>   |<span data-ttu-id="ff31b-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff31b-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff31b-147">memberOf</span><span class="sxs-lookup"><span data-stu-id="ff31b-147">memberOf</span></span>|<span data-ttu-id="ff31b-148">coleção de [conectores](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="ff31b-148">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="ff31b-149">O MemberGroup do qual o conector é membro.</span><span class="sxs-lookup"><span data-stu-id="ff31b-149">The connectorGroup that the connector is a member of.</span></span> <span data-ttu-id="ff31b-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff31b-150">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ff31b-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff31b-151">JSON representation</span></span>

<span data-ttu-id="ff31b-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff31b-152">The following is a JSON representation of the resource.</span></span>

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


