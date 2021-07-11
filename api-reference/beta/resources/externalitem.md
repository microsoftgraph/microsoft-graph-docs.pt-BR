---
title: Tipo de recurso externalItem
description: Um item adicionado a uma conexão Graph Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7c570a7e4754724ca4239b7e3dbe128d09db9d75
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366524"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="1fa59-103">Tipo de recurso externalItem</span><span class="sxs-lookup"><span data-stu-id="1fa59-103">externalItem resource type</span></span>

<span data-ttu-id="1fa59-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fa59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fa59-105">Um item adicionado a uma conexão microsoft Graph [.](externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="1fa59-105">An item added to a Microsoft Graph [connection](externalconnection.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="1fa59-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="1fa59-106">Methods</span></span>

| <span data-ttu-id="1fa59-107">Método</span><span class="sxs-lookup"><span data-stu-id="1fa59-107">Method</span></span>                                                        | <span data-ttu-id="1fa59-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1fa59-108">Return Type</span></span>                     | <span data-ttu-id="1fa59-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fa59-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="1fa59-110">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="1fa59-110">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="1fa59-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="1fa59-111">externalItem</span></span>](externalitem.md) | <span data-ttu-id="1fa59-112">Crie um externalItem.</span><span class="sxs-lookup"><span data-stu-id="1fa59-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="1fa59-113">Obter externalItem</span><span class="sxs-lookup"><span data-stu-id="1fa59-113">Get externalItem</span></span>](../api/externalitem-get.md)                | [<span data-ttu-id="1fa59-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="1fa59-114">externalItem</span></span>](externalitem.md) | <span data-ttu-id="1fa59-115">Obter um externalItem.</span><span class="sxs-lookup"><span data-stu-id="1fa59-115">Get an externalItem.</span></span>    |
| [<span data-ttu-id="1fa59-116">Atualizar externalItem</span><span class="sxs-lookup"><span data-stu-id="1fa59-116">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="1fa59-117">externalItem</span><span class="sxs-lookup"><span data-stu-id="1fa59-117">externalItem</span></span>](externalitem.md) | <span data-ttu-id="1fa59-118">Atualize um externalItem.</span><span class="sxs-lookup"><span data-stu-id="1fa59-118">Update an externalItem.</span></span> |
| [<span data-ttu-id="1fa59-119">Excluir externalItem</span><span class="sxs-lookup"><span data-stu-id="1fa59-119">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="1fa59-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1fa59-120">None</span></span>                            | <span data-ttu-id="1fa59-121">Exclua um externalItem.</span><span class="sxs-lookup"><span data-stu-id="1fa59-121">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="1fa59-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1fa59-122">Properties</span></span>

| <span data-ttu-id="1fa59-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1fa59-123">Property</span></span>   | <span data-ttu-id="1fa59-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fa59-124">Type</span></span>                     | <span data-ttu-id="1fa59-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fa59-125">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="1fa59-126">acl</span><span class="sxs-lookup"><span data-stu-id="1fa59-126">acl</span></span>        | <span data-ttu-id="1fa59-127">[Coleção acl](acl.md)</span><span class="sxs-lookup"><span data-stu-id="1fa59-127">[acl](acl.md) collection</span></span> | <span data-ttu-id="1fa59-128">Uma matriz de entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="1fa59-128">An array of access control entries.</span></span> <span data-ttu-id="1fa59-129">Cada entrada especifica o acesso concedido a um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="1fa59-129">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="1fa59-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fa59-130">Required.</span></span> |
| <span data-ttu-id="1fa59-131">conteúdo</span><span class="sxs-lookup"><span data-stu-id="1fa59-131">content</span></span>    | [<span data-ttu-id="1fa59-132">externalItemContent</span><span class="sxs-lookup"><span data-stu-id="1fa59-132">externalItemContent</span></span>](externalitemcontent.md) | <span data-ttu-id="1fa59-133">Uma representação em texto sem texto do conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="1fa59-133">A plain-text  representation of the contents of the item.</span></span> <span data-ttu-id="1fa59-134">O texto nesta propriedade é indexado em texto completo.</span><span class="sxs-lookup"><span data-stu-id="1fa59-134">The text in this property is full-text indexed.</span></span> <span data-ttu-id="1fa59-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1fa59-135">Optional.</span></span> |
| <span data-ttu-id="1fa59-136">id</span><span class="sxs-lookup"><span data-stu-id="1fa59-136">id</span></span>         | <span data-ttu-id="1fa59-137">String</span><span class="sxs-lookup"><span data-stu-id="1fa59-137">String</span></span>                   | <span data-ttu-id="1fa59-138">ID exclusiva fornecida pelo desenvolvedor do item dentro do [externalConnection](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="1fa59-138">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="1fa59-139">Deve ser alfanumérico e um máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="1fa59-139">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="1fa59-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fa59-140">Required.</span></span> |
| <span data-ttu-id="1fa59-141">properties</span><span class="sxs-lookup"><span data-stu-id="1fa59-141">properties</span></span> | <span data-ttu-id="1fa59-142">Objeto</span><span class="sxs-lookup"><span data-stu-id="1fa59-142">Object</span></span>                   | <span data-ttu-id="1fa59-143">Um pacote de propriedades com as propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="1fa59-143">A property bag with the properties of the item.</span></span> <span data-ttu-id="1fa59-144">As propriedades DEVEM estar em conformidade [com o esquema](schema.md) definido para [externalConnection](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="1fa59-144">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="1fa59-145">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fa59-145">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1fa59-146">Relações</span><span class="sxs-lookup"><span data-stu-id="1fa59-146">Relationships</span></span>

<span data-ttu-id="1fa59-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1fa59-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1fa59-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1fa59-148">JSON representation</span></span>

<span data-ttu-id="1fa59-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1fa59-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItem",
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
