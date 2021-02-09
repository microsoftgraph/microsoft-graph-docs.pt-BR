---
title: Tipo de recurso externalItem
description: Um item adicionado a uma conexão do Microsoft Graph.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 63f0285427a17280169d31a35c3a622d38a6a8c6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161695"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="bd47d-103">Tipo de recurso externalItem</span><span class="sxs-lookup"><span data-stu-id="bd47d-103">externalItem resource type</span></span>

<span data-ttu-id="bd47d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd47d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd47d-105">Um item adicionado a uma conexão [do](externalconnection.md)Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bd47d-105">An item added to a Microsoft Graph [connection](externalconnection.md).</span></span> 

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="bd47d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="bd47d-106">Methods</span></span>

| <span data-ttu-id="bd47d-107">Método</span><span class="sxs-lookup"><span data-stu-id="bd47d-107">Method</span></span>                                                        | <span data-ttu-id="bd47d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bd47d-108">Return Type</span></span>                     | <span data-ttu-id="bd47d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd47d-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="bd47d-110">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="bd47d-110">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="bd47d-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="bd47d-111">externalItem</span></span>](externalitem.md) | <span data-ttu-id="bd47d-112">Crie um externalItem.</span><span class="sxs-lookup"><span data-stu-id="bd47d-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="bd47d-113">Obter externalItem</span><span class="sxs-lookup"><span data-stu-id="bd47d-113">Get externalItem</span></span>](../api/externalitem-get.md)                | [<span data-ttu-id="bd47d-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="bd47d-114">externalItem</span></span>](externalitem.md) | <span data-ttu-id="bd47d-115">Obter um externalItem.</span><span class="sxs-lookup"><span data-stu-id="bd47d-115">Get an externalItem.</span></span>    |
| [<span data-ttu-id="bd47d-116">Atualizar externalItem</span><span class="sxs-lookup"><span data-stu-id="bd47d-116">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="bd47d-117">externalItem</span><span class="sxs-lookup"><span data-stu-id="bd47d-117">externalItem</span></span>](externalitem.md) | <span data-ttu-id="bd47d-118">Atualize um externalItem.</span><span class="sxs-lookup"><span data-stu-id="bd47d-118">Update an externalItem.</span></span> |
| [<span data-ttu-id="bd47d-119">Excluir externalItem</span><span class="sxs-lookup"><span data-stu-id="bd47d-119">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="bd47d-120">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="bd47d-120">None</span></span>                            | <span data-ttu-id="bd47d-121">Exclua um externalItem.</span><span class="sxs-lookup"><span data-stu-id="bd47d-121">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="bd47d-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bd47d-122">Properties</span></span>

| <span data-ttu-id="bd47d-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd47d-123">Property</span></span>   | <span data-ttu-id="bd47d-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd47d-124">Type</span></span>                     | <span data-ttu-id="bd47d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd47d-125">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="bd47d-126">acl</span><span class="sxs-lookup"><span data-stu-id="bd47d-126">acl</span></span>        | <span data-ttu-id="bd47d-127">[coleção acl](acl.md)</span><span class="sxs-lookup"><span data-stu-id="bd47d-127">[acl](acl.md) collection</span></span> | <span data-ttu-id="bd47d-128">Uma matriz de entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="bd47d-128">An array of access control entries.</span></span> <span data-ttu-id="bd47d-129">Cada entrada especifica o acesso concedido a um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="bd47d-129">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="bd47d-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd47d-130">Required.</span></span> |
| <span data-ttu-id="bd47d-131">conteúdo</span><span class="sxs-lookup"><span data-stu-id="bd47d-131">content</span></span>    | [<span data-ttu-id="bd47d-132">externalItemContent</span><span class="sxs-lookup"><span data-stu-id="bd47d-132">externalItemContent</span></span>](externalitemcontent.md) | <span data-ttu-id="bd47d-133">Uma representação em texto sem texto do conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="bd47d-133">A plain-text  representation of the contents of the item.</span></span> <span data-ttu-id="bd47d-134">O texto nesta propriedade é indexado em texto completo.</span><span class="sxs-lookup"><span data-stu-id="bd47d-134">The text in this property is full-text indexed.</span></span> <span data-ttu-id="bd47d-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="bd47d-135">Optional.</span></span> |
| <span data-ttu-id="bd47d-136">id</span><span class="sxs-lookup"><span data-stu-id="bd47d-136">id</span></span>         | <span data-ttu-id="bd47d-137">String</span><span class="sxs-lookup"><span data-stu-id="bd47d-137">String</span></span>                   | <span data-ttu-id="bd47d-138">ID exclusiva fornecida pelo desenvolvedor do item dentro do [externalConnection que o contém.](externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="bd47d-138">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="bd47d-139">Deve ser alfanumérico e um máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="bd47d-139">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="bd47d-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd47d-140">Required.</span></span> |
| <span data-ttu-id="bd47d-141">properties</span><span class="sxs-lookup"><span data-stu-id="bd47d-141">properties</span></span> | <span data-ttu-id="bd47d-142">Objeto</span><span class="sxs-lookup"><span data-stu-id="bd47d-142">Object</span></span>                   | <span data-ttu-id="bd47d-143">Um pacote de propriedades com as propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="bd47d-143">A property bag with the properties of the item.</span></span> <span data-ttu-id="bd47d-144">As propriedades DEVEM estar em conformidade [com o esquema](schema.md) definido para [externalConnection](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="bd47d-144">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="bd47d-145">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd47d-145">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bd47d-146">Relações</span><span class="sxs-lookup"><span data-stu-id="bd47d-146">Relationships</span></span>

<span data-ttu-id="bd47d-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bd47d-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd47d-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bd47d-148">JSON representation</span></span>

<span data-ttu-id="bd47d-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bd47d-149">The following is a JSON representation of the resource.</span></span>

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
