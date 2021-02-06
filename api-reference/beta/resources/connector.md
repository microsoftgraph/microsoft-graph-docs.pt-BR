---
title: tipo de recurso do conector
description: Representa um conector de Proxy de Aplicativo.
author: japere
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 53a5726456ce3d03ea537e87ec0dddb901623601
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136767"
---
# <a name="connector-resource-type"></a><span data-ttu-id="5cb8e-103">tipo de recurso do conector</span><span class="sxs-lookup"><span data-stu-id="5cb8e-103">connector resource type</span></span>

<span data-ttu-id="5cb8e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cb8e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cb8e-105">Conectores são agentes leves que ficam no local e facilitam a conexão de saída com o serviço de Proxy de Aplicativo do [Azure AD.](https://aka.ms/whyappproxy)</span><span class="sxs-lookup"><span data-stu-id="5cb8e-105">Connectors are lightweight agents that sit on-premises and facilitate the outbound connection to the [Azure AD Application Proxy](https://aka.ms/whyappproxy) service.</span></span> <span data-ttu-id="5cb8e-106">Cada conector faz parte de um [connectorGroup](connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="5cb8e-106">Each connector is part of a [connectorGroup](connectorgroup.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5cb8e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="5cb8e-107">Methods</span></span>

| <span data-ttu-id="5cb8e-108">Método</span><span class="sxs-lookup"><span data-stu-id="5cb8e-108">Method</span></span>       | <span data-ttu-id="5cb8e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5cb8e-109">Return Type</span></span> | <span data-ttu-id="5cb8e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cb8e-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5cb8e-111">Listar conectores</span><span class="sxs-lookup"><span data-stu-id="5cb8e-111">List connectors</span></span>](../api/connector-list.md) | <span data-ttu-id="5cb8e-112">[conjunto de conectores](connector.md)</span><span class="sxs-lookup"><span data-stu-id="5cb8e-112">[connector](connector.md) collection</span></span> | <span data-ttu-id="5cb8e-113">Recupere uma lista de objetos de conector.</span><span class="sxs-lookup"><span data-stu-id="5cb8e-113">Retrieve a list of connector objects.</span></span> | 
| [<span data-ttu-id="5cb8e-114">Obter conector</span><span class="sxs-lookup"><span data-stu-id="5cb8e-114">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="5cb8e-115">connector</span><span class="sxs-lookup"><span data-stu-id="5cb8e-115">connector</span></span>](connector.md) | <span data-ttu-id="5cb8e-116">Leia as propriedades e os relacionamentos do objeto connector.</span><span class="sxs-lookup"><span data-stu-id="5cb8e-116">Read properties and relationships of connector object.</span></span> |
| [<span data-ttu-id="5cb8e-117">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="5cb8e-117">List memberOf</span></span>](../api/connector-list-memberof.md) | <span data-ttu-id="5cb8e-118">[Coleção connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="5cb8e-118">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="5cb8e-119">Listar a coleção de objetos connectorGroup da que o conector é membro.</span><span class="sxs-lookup"><span data-stu-id="5cb8e-119">List the connectorGroup object collection the connector is a member of.</span></span> |
| [<span data-ttu-id="5cb8e-120">Adicionar conector a connectorGroup</span><span class="sxs-lookup"><span data-stu-id="5cb8e-120">Add connector to connectorGroup</span></span>](../api/connector-post-memberof.md)| [<span data-ttu-id="5cb8e-121">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="5cb8e-121">connectorGroup</span></span>](connectorgroup.md) | <span data-ttu-id="5cb8e-122">Adicione um conector a um connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="5cb8e-122">Add a connector to a connectorGroup.</span></span> |


## <a name="properties"></a><span data-ttu-id="5cb8e-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5cb8e-123">Properties</span></span>
| <span data-ttu-id="5cb8e-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5cb8e-124">Property</span></span>     | <span data-ttu-id="5cb8e-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="5cb8e-125">Type</span></span>        | <span data-ttu-id="5cb8e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cb8e-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5cb8e-127">externalIp</span><span class="sxs-lookup"><span data-stu-id="5cb8e-127">externalIp</span></span>|<span data-ttu-id="5cb8e-128">String</span><span class="sxs-lookup"><span data-stu-id="5cb8e-128">String</span></span>| <span data-ttu-id="5cb8e-129">O endereço IP externo detectado pelo servidor do conector.</span><span class="sxs-lookup"><span data-stu-id="5cb8e-129">The external IP address as detected by the the connector server.</span></span> <span data-ttu-id="5cb8e-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5cb8e-130">Read-only.</span></span> |
|<span data-ttu-id="5cb8e-131">id</span><span class="sxs-lookup"><span data-stu-id="5cb8e-131">id</span></span>|<span data-ttu-id="5cb8e-132">String</span><span class="sxs-lookup"><span data-stu-id="5cb8e-132">String</span></span>| <span data-ttu-id="5cb8e-133">Identificador exclusivo do conector.</span><span class="sxs-lookup"><span data-stu-id="5cb8e-133">Unique identifier of the connector.</span></span> <span data-ttu-id="5cb8e-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5cb8e-134">Read-only.</span></span> |
|<span data-ttu-id="5cb8e-135">machineName</span><span class="sxs-lookup"><span data-stu-id="5cb8e-135">machineName</span></span>|<span data-ttu-id="5cb8e-136">String</span><span class="sxs-lookup"><span data-stu-id="5cb8e-136">String</span></span>| <span data-ttu-id="5cb8e-137">O nome do computador em que o conector está instalado e em execução.</span><span class="sxs-lookup"><span data-stu-id="5cb8e-137">The machine name the connector is installed and running on.</span></span> |
|<span data-ttu-id="5cb8e-138">status</span><span class="sxs-lookup"><span data-stu-id="5cb8e-138">status</span></span>|<span data-ttu-id="5cb8e-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5cb8e-139">string</span></span>| <span data-ttu-id="5cb8e-140">Indica o status do conector.</span><span class="sxs-lookup"><span data-stu-id="5cb8e-140">Indicates the status of the connector.</span></span> <span data-ttu-id="5cb8e-141">Os valores possíveis são: `active` e `inactive`.</span><span class="sxs-lookup"><span data-stu-id="5cb8e-141">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="5cb8e-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5cb8e-142">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5cb8e-143">Relações</span><span class="sxs-lookup"><span data-stu-id="5cb8e-143">Relationships</span></span>
| <span data-ttu-id="5cb8e-144">Relação</span><span class="sxs-lookup"><span data-stu-id="5cb8e-144">Relationship</span></span> | <span data-ttu-id="5cb8e-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="5cb8e-145">Type</span></span>   |<span data-ttu-id="5cb8e-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cb8e-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cb8e-147">memberOf</span><span class="sxs-lookup"><span data-stu-id="5cb8e-147">memberOf</span></span>|<span data-ttu-id="5cb8e-148">[Coleção connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="5cb8e-148">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="5cb8e-149">O connectorGroup do que o conector é membro.</span><span class="sxs-lookup"><span data-stu-id="5cb8e-149">The connectorGroup that the connector is a member of.</span></span> <span data-ttu-id="5cb8e-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5cb8e-150">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5cb8e-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5cb8e-151">JSON representation</span></span>

<span data-ttu-id="5cb8e-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5cb8e-152">The following is a JSON representation of the resource.</span></span>

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



