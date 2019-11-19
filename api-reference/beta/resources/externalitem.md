---
title: tipo de recurso externalItem
description: Um item indexado por meio de uma conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 900cf61536204ff5924aea0de268befad6626b37
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704168"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="a792b-103">tipo de recurso externalItem</span><span class="sxs-lookup"><span data-stu-id="a792b-103">externalItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a792b-104">Um item indexado por meio de uma [conexão](externalconnection.md)de pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a792b-104">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="a792b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="a792b-105">Methods</span></span>

| <span data-ttu-id="a792b-106">Método</span><span class="sxs-lookup"><span data-stu-id="a792b-106">Method</span></span>                                                        | <span data-ttu-id="a792b-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a792b-107">Return Type</span></span>                     | <span data-ttu-id="a792b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a792b-108">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="a792b-109">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="a792b-109">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="a792b-110">externalItem</span><span class="sxs-lookup"><span data-stu-id="a792b-110">externalItem</span></span>](externalitem.md) | <span data-ttu-id="a792b-111">Criar um externalItem.</span><span class="sxs-lookup"><span data-stu-id="a792b-111">Create an externalItem.</span></span> |
| [<span data-ttu-id="a792b-112">Atualizar externalItem</span><span class="sxs-lookup"><span data-stu-id="a792b-112">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="a792b-113">externalItem</span><span class="sxs-lookup"><span data-stu-id="a792b-113">externalItem</span></span>](externalitem.md) | <span data-ttu-id="a792b-114">Atualizar um externalItem.</span><span class="sxs-lookup"><span data-stu-id="a792b-114">Update an externalItem.</span></span> |
| [<span data-ttu-id="a792b-115">Excluir externalItem</span><span class="sxs-lookup"><span data-stu-id="a792b-115">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="a792b-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a792b-116">None</span></span>                            | <span data-ttu-id="a792b-117">Excluir um externalItem.</span><span class="sxs-lookup"><span data-stu-id="a792b-117">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="a792b-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a792b-118">Properties</span></span>

| <span data-ttu-id="a792b-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a792b-119">Property</span></span>   | <span data-ttu-id="a792b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a792b-120">Type</span></span>                     | <span data-ttu-id="a792b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a792b-121">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="a792b-122">ACL</span><span class="sxs-lookup"><span data-stu-id="a792b-122">acl</span></span>        | <span data-ttu-id="a792b-123">coleção [ACL](acl.md)</span><span class="sxs-lookup"><span data-stu-id="a792b-123">[acl](acl.md) collection</span></span> | <span data-ttu-id="a792b-124">Uma matriz de entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="a792b-124">An array of access control entries.</span></span> <span data-ttu-id="a792b-125">Cada entrada especifica o acesso concedido a um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="a792b-125">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="a792b-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a792b-126">Required.</span></span> |
| <span data-ttu-id="a792b-127">content</span><span class="sxs-lookup"><span data-stu-id="a792b-127">content</span></span>    | <span data-ttu-id="a792b-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a792b-128">String</span></span>                   | <span data-ttu-id="a792b-129">Uma representação de texto simples do conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="a792b-129">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="a792b-130">O texto nessa propriedade é indexado de texto completo.</span><span class="sxs-lookup"><span data-stu-id="a792b-130">The text in this property is full-text indexed.</span></span> <span data-ttu-id="a792b-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a792b-131">Optional.</span></span> |
| <span data-ttu-id="a792b-132">id</span><span class="sxs-lookup"><span data-stu-id="a792b-132">id</span></span>         | <span data-ttu-id="a792b-133">String</span><span class="sxs-lookup"><span data-stu-id="a792b-133">String</span></span>                   | <span data-ttu-id="a792b-134">ID exclusiva fornecida pelo desenvolvedor do item dentro do [externalConnection](externalconnection.md)que contém o.</span><span class="sxs-lookup"><span data-stu-id="a792b-134">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="a792b-135">Deve ser alfanumérico e um máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="a792b-135">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="a792b-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a792b-136">Required.</span></span> |
| <span data-ttu-id="a792b-137">properties</span><span class="sxs-lookup"><span data-stu-id="a792b-137">properties</span></span> | <span data-ttu-id="a792b-138">Objeto</span><span class="sxs-lookup"><span data-stu-id="a792b-138">Object</span></span>                   | <span data-ttu-id="a792b-139">Um recipiente de propriedades com as propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="a792b-139">A property bag with the properties of the item.</span></span> <span data-ttu-id="a792b-140">As propriedades devem estar em conformidade com o [esquema](schema.md) definido para o [externalConnection](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="a792b-140">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="a792b-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a792b-141">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a792b-142">Relações</span><span class="sxs-lookup"><span data-stu-id="a792b-142">Relationships</span></span>

<span data-ttu-id="a792b-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a792b-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a792b-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a792b-144">JSON representation</span></span>

<span data-ttu-id="a792b-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a792b-145">The following is a JSON representation of the resource.</span></span>

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
  "content": "String",
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
