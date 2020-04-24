---
title: tipo de recurso externalItem
description: Um item indexado por meio de uma conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e1497528e759a2fb5556aed3e9b936b1c9797ee0
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805656"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="c9d2d-103">tipo de recurso externalItem</span><span class="sxs-lookup"><span data-stu-id="c9d2d-103">externalItem resource type</span></span>

<span data-ttu-id="c9d2d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9d2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9d2d-105">Um item indexado por meio de uma [conexão](externalconnection.md)de pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c9d2d-105">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="c9d2d-106">Methods</span><span class="sxs-lookup"><span data-stu-id="c9d2d-106">Methods</span></span>

| <span data-ttu-id="c9d2d-107">Método</span><span class="sxs-lookup"><span data-stu-id="c9d2d-107">Method</span></span>                                                        | <span data-ttu-id="c9d2d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c9d2d-108">Return Type</span></span>                     | <span data-ttu-id="c9d2d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9d2d-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="c9d2d-110">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="c9d2d-110">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="c9d2d-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="c9d2d-111">externalItem</span></span>](externalitem.md) | <span data-ttu-id="c9d2d-112">Criar um externalItem.</span><span class="sxs-lookup"><span data-stu-id="c9d2d-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="c9d2d-113">Atualizar externalItem</span><span class="sxs-lookup"><span data-stu-id="c9d2d-113">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="c9d2d-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="c9d2d-114">externalItem</span></span>](externalitem.md) | <span data-ttu-id="c9d2d-115">Atualizar um externalItem.</span><span class="sxs-lookup"><span data-stu-id="c9d2d-115">Update an externalItem.</span></span> |
| [<span data-ttu-id="c9d2d-116">Excluir externalItem</span><span class="sxs-lookup"><span data-stu-id="c9d2d-116">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="c9d2d-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c9d2d-117">None</span></span>                            | <span data-ttu-id="c9d2d-118">Excluir um externalItem.</span><span class="sxs-lookup"><span data-stu-id="c9d2d-118">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="c9d2d-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9d2d-119">Properties</span></span>

| <span data-ttu-id="c9d2d-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9d2d-120">Property</span></span>   | <span data-ttu-id="c9d2d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9d2d-121">Type</span></span>                     | <span data-ttu-id="c9d2d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9d2d-122">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="c9d2d-123">ACL</span><span class="sxs-lookup"><span data-stu-id="c9d2d-123">acl</span></span>        | <span data-ttu-id="c9d2d-124">coleção [ACL](acl.md)</span><span class="sxs-lookup"><span data-stu-id="c9d2d-124">[acl](acl.md) collection</span></span> | <span data-ttu-id="c9d2d-125">Uma matriz de entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="c9d2d-125">An array of access control entries.</span></span> <span data-ttu-id="c9d2d-126">Cada entrada especifica o acesso concedido a um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="c9d2d-126">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="c9d2d-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9d2d-127">Required.</span></span> |
| <span data-ttu-id="c9d2d-128">conteúdo</span><span class="sxs-lookup"><span data-stu-id="c9d2d-128">content</span></span>    | [<span data-ttu-id="c9d2d-129">externalItemContent</span><span class="sxs-lookup"><span data-stu-id="c9d2d-129">externalItemContent</span></span>](externalitemcontent.md) | <span data-ttu-id="c9d2d-130">Uma representação de texto sem formatação ou HTML do conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="c9d2d-130">A plain-text or HTML representation of the contents of the item.</span></span> <span data-ttu-id="c9d2d-131">O texto nessa propriedade é indexado de texto completo.</span><span class="sxs-lookup"><span data-stu-id="c9d2d-131">The text in this property is full-text indexed.</span></span> <span data-ttu-id="c9d2d-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c9d2d-132">Optional.</span></span> |
| <span data-ttu-id="c9d2d-133">id</span><span class="sxs-lookup"><span data-stu-id="c9d2d-133">id</span></span>         | <span data-ttu-id="c9d2d-134">String</span><span class="sxs-lookup"><span data-stu-id="c9d2d-134">String</span></span>                   | <span data-ttu-id="c9d2d-135">ID exclusiva fornecida pelo desenvolvedor do item dentro do [externalConnection](externalconnection.md)que contém o.</span><span class="sxs-lookup"><span data-stu-id="c9d2d-135">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="c9d2d-136">Deve ser alfanumérico e um máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="c9d2d-136">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="c9d2d-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9d2d-137">Required.</span></span> |
| <span data-ttu-id="c9d2d-138">properties</span><span class="sxs-lookup"><span data-stu-id="c9d2d-138">properties</span></span> | <span data-ttu-id="c9d2d-139">Objeto</span><span class="sxs-lookup"><span data-stu-id="c9d2d-139">Object</span></span>                   | <span data-ttu-id="c9d2d-140">Um recipiente de propriedades com as propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="c9d2d-140">A property bag with the properties of the item.</span></span> <span data-ttu-id="c9d2d-141">As propriedades devem estar em conformidade com o [esquema](schema.md) definido para o [externalConnection](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="c9d2d-141">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="c9d2d-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9d2d-142">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c9d2d-143">Relações</span><span class="sxs-lookup"><span data-stu-id="c9d2d-143">Relationships</span></span>

<span data-ttu-id="c9d2d-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c9d2d-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9d2d-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9d2d-145">JSON representation</span></span>

<span data-ttu-id="c9d2d-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c9d2d-146">The following is a JSON representation of the resource.</span></span>

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
