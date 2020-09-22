---
title: tipo de recurso externalItem
description: Um item indexado por meio de uma conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: d775cfefa7a0cd1fdb87a291ba7ac61bb4b40782
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013699"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="ed1c0-103">tipo de recurso externalItem</span><span class="sxs-lookup"><span data-stu-id="ed1c0-103">externalItem resource type</span></span>

<span data-ttu-id="ed1c0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed1c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed1c0-105">Um item indexado por meio de uma [conexão](externalconnection.md)de pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ed1c0-105">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="ed1c0-106">Methods</span><span class="sxs-lookup"><span data-stu-id="ed1c0-106">Methods</span></span>

| <span data-ttu-id="ed1c0-107">Método</span><span class="sxs-lookup"><span data-stu-id="ed1c0-107">Method</span></span>                                                        | <span data-ttu-id="ed1c0-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ed1c0-108">Return Type</span></span>                     | <span data-ttu-id="ed1c0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed1c0-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="ed1c0-110">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="ed1c0-110">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="ed1c0-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="ed1c0-111">externalItem</span></span>](externalitem.md) | <span data-ttu-id="ed1c0-112">Criar um externalItem.</span><span class="sxs-lookup"><span data-stu-id="ed1c0-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="ed1c0-113">Obter externalItem</span><span class="sxs-lookup"><span data-stu-id="ed1c0-113">Get externalItem</span></span>](../api/externalitem-get.md)                | [<span data-ttu-id="ed1c0-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="ed1c0-114">externalItem</span></span>](externalitem.md) | <span data-ttu-id="ed1c0-115">Obter um externalItem.</span><span class="sxs-lookup"><span data-stu-id="ed1c0-115">Get an externalItem.</span></span>    |
| [<span data-ttu-id="ed1c0-116">Atualizar externalItem</span><span class="sxs-lookup"><span data-stu-id="ed1c0-116">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="ed1c0-117">externalItem</span><span class="sxs-lookup"><span data-stu-id="ed1c0-117">externalItem</span></span>](externalitem.md) | <span data-ttu-id="ed1c0-118">Atualizar um externalItem.</span><span class="sxs-lookup"><span data-stu-id="ed1c0-118">Update an externalItem.</span></span> |
| [<span data-ttu-id="ed1c0-119">Excluir externalItem</span><span class="sxs-lookup"><span data-stu-id="ed1c0-119">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="ed1c0-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed1c0-120">None</span></span>                            | <span data-ttu-id="ed1c0-121">Excluir um externalItem.</span><span class="sxs-lookup"><span data-stu-id="ed1c0-121">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="ed1c0-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed1c0-122">Properties</span></span>

| <span data-ttu-id="ed1c0-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed1c0-123">Property</span></span>   | <span data-ttu-id="ed1c0-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed1c0-124">Type</span></span>                     | <span data-ttu-id="ed1c0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed1c0-125">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="ed1c0-126">ACL</span><span class="sxs-lookup"><span data-stu-id="ed1c0-126">acl</span></span>        | <span data-ttu-id="ed1c0-127">coleção [ACL](acl.md)</span><span class="sxs-lookup"><span data-stu-id="ed1c0-127">[acl](acl.md) collection</span></span> | <span data-ttu-id="ed1c0-128">Uma matriz de entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="ed1c0-128">An array of access control entries.</span></span> <span data-ttu-id="ed1c0-129">Cada entrada especifica o acesso concedido a um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="ed1c0-129">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="ed1c0-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed1c0-130">Required.</span></span> |
| <span data-ttu-id="ed1c0-131">conteúdo</span><span class="sxs-lookup"><span data-stu-id="ed1c0-131">content</span></span>    | [<span data-ttu-id="ed1c0-132">externalItemContent</span><span class="sxs-lookup"><span data-stu-id="ed1c0-132">externalItemContent</span></span>](externalitemcontent.md) | <span data-ttu-id="ed1c0-133">Uma representação de texto sem formatação ou HTML do conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="ed1c0-133">A plain-text or HTML representation of the contents of the item.</span></span> <span data-ttu-id="ed1c0-134">O texto nessa propriedade é indexado de texto completo.</span><span class="sxs-lookup"><span data-stu-id="ed1c0-134">The text in this property is full-text indexed.</span></span> <span data-ttu-id="ed1c0-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ed1c0-135">Optional.</span></span> |
| <span data-ttu-id="ed1c0-136">id</span><span class="sxs-lookup"><span data-stu-id="ed1c0-136">id</span></span>         | <span data-ttu-id="ed1c0-137">String</span><span class="sxs-lookup"><span data-stu-id="ed1c0-137">String</span></span>                   | <span data-ttu-id="ed1c0-138">ID exclusiva fornecida pelo desenvolvedor do item dentro do [externalConnection](externalconnection.md)que contém o.</span><span class="sxs-lookup"><span data-stu-id="ed1c0-138">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="ed1c0-139">Deve ser alfanumérico e um máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="ed1c0-139">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="ed1c0-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed1c0-140">Required.</span></span> |
| <span data-ttu-id="ed1c0-141">properties</span><span class="sxs-lookup"><span data-stu-id="ed1c0-141">properties</span></span> | <span data-ttu-id="ed1c0-142">Objeto</span><span class="sxs-lookup"><span data-stu-id="ed1c0-142">Object</span></span>                   | <span data-ttu-id="ed1c0-143">Um recipiente de propriedades com as propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="ed1c0-143">A property bag with the properties of the item.</span></span> <span data-ttu-id="ed1c0-144">As propriedades devem estar em conformidade com o [esquema](schema.md) definido para o [externalConnection](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="ed1c0-144">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="ed1c0-145">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed1c0-145">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ed1c0-146">Relações</span><span class="sxs-lookup"><span data-stu-id="ed1c0-146">Relationships</span></span>

<span data-ttu-id="ed1c0-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed1c0-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed1c0-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed1c0-148">JSON representation</span></span>

<span data-ttu-id="ed1c0-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed1c0-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItem",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "acl": [{"@odata.type": "microsoft.graph.acl"}],
  "content": {"@odata.type": "microsoft.graph.externalItemContent"},
  "id": "String (identifier)",
  "properties": "Object"
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
    "Error: microsoft.graph.externalItem/properties:\r\n      Referenced type microsoft.graph.object is not defined in the doc set! Potential suggestion: microsoft.graph.directoryObject"
  ]
}-->


