---
title: Tipo de recurso externalItem
description: Um item adicionado a uma conexão Graph Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8660365d5d08d0084066cea3349e841269469241
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467602"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="7903a-103">Tipo de recurso externalItem</span><span class="sxs-lookup"><span data-stu-id="7903a-103">externalItem resource type</span></span>

<span data-ttu-id="7903a-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="7903a-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7903a-105">Um item adicionado a uma conexão microsoft Graph [.](externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="7903a-105">An item added to a Microsoft Graph [connection](externalconnectors-externalconnection.md).</span></span>

## <a name="methods"></a><span data-ttu-id="7903a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="7903a-106">Methods</span></span>

| <span data-ttu-id="7903a-107">Método</span><span class="sxs-lookup"><span data-stu-id="7903a-107">Method</span></span>                                                        | <span data-ttu-id="7903a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7903a-108">Return Type</span></span>                     | <span data-ttu-id="7903a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7903a-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="7903a-110">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="7903a-110">Create externalItem</span></span>](../api/externalconnectors-externalconnection-put-items.md) | [<span data-ttu-id="7903a-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="7903a-111">externalItem</span></span>](externalconnectors-externalitem.md) | <span data-ttu-id="7903a-112">Crie um externalItem.</span><span class="sxs-lookup"><span data-stu-id="7903a-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="7903a-113">Obter externalItem</span><span class="sxs-lookup"><span data-stu-id="7903a-113">Get externalItem</span></span>](../api/externalconnectors-externalitem-get.md)                | [<span data-ttu-id="7903a-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="7903a-114">externalItem</span></span>](externalconnectors-externalitem.md) | <span data-ttu-id="7903a-115">Obter um externalItem.</span><span class="sxs-lookup"><span data-stu-id="7903a-115">Get an externalItem.</span></span>    |
| [<span data-ttu-id="7903a-116">Atualizar externalItem</span><span class="sxs-lookup"><span data-stu-id="7903a-116">Update externalItem</span></span>](../api/externalconnectors-externalitem-update.md)          | [<span data-ttu-id="7903a-117">externalItem</span><span class="sxs-lookup"><span data-stu-id="7903a-117">externalItem</span></span>](externalconnectors-externalitem.md) | <span data-ttu-id="7903a-118">Atualize um externalItem.</span><span class="sxs-lookup"><span data-stu-id="7903a-118">Update an externalItem.</span></span> |
| [<span data-ttu-id="7903a-119">Excluir externalItem</span><span class="sxs-lookup"><span data-stu-id="7903a-119">Delete externalItem</span></span>](../api/externalconnectors-externalitem-delete.md)          | <span data-ttu-id="7903a-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7903a-120">None</span></span>                            | <span data-ttu-id="7903a-121">Exclua um externalItem.</span><span class="sxs-lookup"><span data-stu-id="7903a-121">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="7903a-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7903a-122">Properties</span></span>

| <span data-ttu-id="7903a-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7903a-123">Property</span></span>   | <span data-ttu-id="7903a-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="7903a-124">Type</span></span>                     | <span data-ttu-id="7903a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7903a-125">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="7903a-126">acl</span><span class="sxs-lookup"><span data-stu-id="7903a-126">acl</span></span>        | <span data-ttu-id="7903a-127">[Coleção microsoft.graph.externalConnectors.acl](externalconnectors-acl.md)</span><span class="sxs-lookup"><span data-stu-id="7903a-127">[microsoft.graph.externalConnectors.acl](externalconnectors-acl.md) collection</span></span> | <span data-ttu-id="7903a-128">Uma matriz de entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="7903a-128">An array of access control entries.</span></span> <span data-ttu-id="7903a-129">Cada entrada especifica o acesso concedido a um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="7903a-129">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="7903a-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7903a-130">Required.</span></span> |
| <span data-ttu-id="7903a-131">conteúdo</span><span class="sxs-lookup"><span data-stu-id="7903a-131">content</span></span>    | [<span data-ttu-id="7903a-132">microsoft.graph.externalConnectors.externalItemContent</span><span class="sxs-lookup"><span data-stu-id="7903a-132">microsoft.graph.externalConnectors.externalItemContent</span></span>](externalconnectors-externalitemcontent.md) | <span data-ttu-id="7903a-133">Uma representação em texto sem texto do conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="7903a-133">A plain-text  representation of the contents of the item.</span></span> <span data-ttu-id="7903a-134">O texto nesta propriedade é indexado em texto completo.</span><span class="sxs-lookup"><span data-stu-id="7903a-134">The text in this property is full-text indexed.</span></span> <span data-ttu-id="7903a-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7903a-135">Optional.</span></span> |
| <span data-ttu-id="7903a-136">id</span><span class="sxs-lookup"><span data-stu-id="7903a-136">id</span></span>         | <span data-ttu-id="7903a-137">String</span><span class="sxs-lookup"><span data-stu-id="7903a-137">String</span></span>                   | <span data-ttu-id="7903a-138">ID exclusiva fornecida pelo desenvolvedor do item dentro do [externalConnection](externalconnectors-externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="7903a-138">Developer-provided unique ID of the item within the containing [externalConnection](externalconnectors-externalconnection.md).</span></span> <span data-ttu-id="7903a-139">Deve ser alfanumérico e um máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="7903a-139">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="7903a-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7903a-140">Required.</span></span> |
| <span data-ttu-id="7903a-141">properties</span><span class="sxs-lookup"><span data-stu-id="7903a-141">properties</span></span> | <span data-ttu-id="7903a-142">Objeto</span><span class="sxs-lookup"><span data-stu-id="7903a-142">Object</span></span>                   | <span data-ttu-id="7903a-143">Um pacote de propriedades com as propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="7903a-143">A property bag with the properties of the item.</span></span> <span data-ttu-id="7903a-144">As propriedades DEVEM estar em conformidade [com o esquema](externalconnectors-schema.md) definido para [externalConnection](externalconnectors-externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="7903a-144">The properties MUST conform to the [schema](externalconnectors-schema.md) defined for the [externalConnection](externalconnectors-externalconnection.md).</span></span> <span data-ttu-id="7903a-145">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7903a-145">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7903a-146">Relações</span><span class="sxs-lookup"><span data-stu-id="7903a-146">Relationships</span></span>

<span data-ttu-id="7903a-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7903a-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7903a-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7903a-148">JSON representation</span></span>

<span data-ttu-id="7903a-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7903a-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.externalConnectors.externalItem",
  "keyProperty": "id"
}-->

```json
{
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    }
  ],
  "id": "String (identifier)",
  "properties": "Object",
  "content": { "@odata.type": "microsoft.graph.externalConnectors.externalItemContent" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: microsoft.graph.externalConnectors.externalItem/properties:\r\n      Referenced type microsoft.graph.object is not defined in the doc set! Potential suggestion: microsoft.graph.directoryObject"
  ]
}-->
