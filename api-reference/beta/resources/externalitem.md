---
title: tipo de recurso externalItem
description: Um item indexado por meio de uma conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e115135bedecfe4b055e028d5c19902a068c8a53
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498697"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="279b5-103">tipo de recurso externalItem</span><span class="sxs-lookup"><span data-stu-id="279b5-103">externalItem resource type</span></span>

<span data-ttu-id="279b5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="279b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="279b5-105">Um item indexado por meio de uma [conexão](externalconnection.md)de pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="279b5-105">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="279b5-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="279b5-106">Methods</span></span>

| <span data-ttu-id="279b5-107">Método</span><span class="sxs-lookup"><span data-stu-id="279b5-107">Method</span></span>                                                        | <span data-ttu-id="279b5-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="279b5-108">Return Type</span></span>                     | <span data-ttu-id="279b5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="279b5-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="279b5-110">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="279b5-110">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="279b5-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="279b5-111">externalItem</span></span>](externalitem.md) | <span data-ttu-id="279b5-112">Criar um externalItem.</span><span class="sxs-lookup"><span data-stu-id="279b5-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="279b5-113">Atualizar externalItem</span><span class="sxs-lookup"><span data-stu-id="279b5-113">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="279b5-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="279b5-114">externalItem</span></span>](externalitem.md) | <span data-ttu-id="279b5-115">Atualizar um externalItem.</span><span class="sxs-lookup"><span data-stu-id="279b5-115">Update an externalItem.</span></span> |
| [<span data-ttu-id="279b5-116">Excluir externalItem</span><span class="sxs-lookup"><span data-stu-id="279b5-116">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="279b5-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="279b5-117">None</span></span>                            | <span data-ttu-id="279b5-118">Excluir um externalItem.</span><span class="sxs-lookup"><span data-stu-id="279b5-118">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="279b5-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="279b5-119">Properties</span></span>

| <span data-ttu-id="279b5-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="279b5-120">Property</span></span>   | <span data-ttu-id="279b5-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="279b5-121">Type</span></span>                     | <span data-ttu-id="279b5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="279b5-122">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="279b5-123">ACL</span><span class="sxs-lookup"><span data-stu-id="279b5-123">acl</span></span>        | <span data-ttu-id="279b5-124">coleção [ACL](acl.md)</span><span class="sxs-lookup"><span data-stu-id="279b5-124">[acl](acl.md) collection</span></span> | <span data-ttu-id="279b5-125">Uma matriz de entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="279b5-125">An array of access control entries.</span></span> <span data-ttu-id="279b5-126">Cada entrada especifica o acesso concedido a um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="279b5-126">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="279b5-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="279b5-127">Required.</span></span> |
| <span data-ttu-id="279b5-128">content</span><span class="sxs-lookup"><span data-stu-id="279b5-128">content</span></span>    | <span data-ttu-id="279b5-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="279b5-129">String</span></span>                   | <span data-ttu-id="279b5-130">Uma representação de texto simples do conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="279b5-130">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="279b5-131">O texto nessa propriedade é indexado de texto completo.</span><span class="sxs-lookup"><span data-stu-id="279b5-131">The text in this property is full-text indexed.</span></span> <span data-ttu-id="279b5-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="279b5-132">Optional.</span></span> |
| <span data-ttu-id="279b5-133">id</span><span class="sxs-lookup"><span data-stu-id="279b5-133">id</span></span>         | <span data-ttu-id="279b5-134">String</span><span class="sxs-lookup"><span data-stu-id="279b5-134">String</span></span>                   | <span data-ttu-id="279b5-135">ID exclusiva fornecida pelo desenvolvedor do item dentro do [externalConnection](externalconnection.md)que contém o.</span><span class="sxs-lookup"><span data-stu-id="279b5-135">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="279b5-136">Deve ser alfanumérico e um máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="279b5-136">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="279b5-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="279b5-137">Required.</span></span> |
| <span data-ttu-id="279b5-138">properties</span><span class="sxs-lookup"><span data-stu-id="279b5-138">properties</span></span> | <span data-ttu-id="279b5-139">Objeto</span><span class="sxs-lookup"><span data-stu-id="279b5-139">Object</span></span>                   | <span data-ttu-id="279b5-140">Um recipiente de propriedades com as propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="279b5-140">A property bag with the properties of the item.</span></span> <span data-ttu-id="279b5-141">As propriedades devem estar em conformidade com o [esquema](schema.md) definido para o [externalConnection](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="279b5-141">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="279b5-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="279b5-142">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="279b5-143">Relações</span><span class="sxs-lookup"><span data-stu-id="279b5-143">Relationships</span></span>

<span data-ttu-id="279b5-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="279b5-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="279b5-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="279b5-145">JSON representation</span></span>

<span data-ttu-id="279b5-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="279b5-146">The following is a JSON representation of the resource.</span></span>

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
