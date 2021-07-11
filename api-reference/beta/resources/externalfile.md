---
title: Tipo de recurso externalFile
description: Um arquivo indexado por meio de Pesquisa da Microsoft conexão.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 23a89cb83e85f16fc4cf2faa3c285bafb9fd66cf
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366545"
---
# <a name="externalfile-resource-type"></a><span data-ttu-id="6a500-103">Tipo de recurso externalFile</span><span class="sxs-lookup"><span data-stu-id="6a500-103">externalFile resource type</span></span>

<span data-ttu-id="6a500-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a500-104">Namespace: microsoft.graph</span></span>

> [!CAUTION]
> <span data-ttu-id="6a500-105">O `externalFile` tipo foi preterido.</span><span class="sxs-lookup"><span data-stu-id="6a500-105">The `externalFile` type has been deprecated.</span></span> <span data-ttu-id="6a500-106">Os desenvolvedores não devem usar esse tipo.</span><span class="sxs-lookup"><span data-stu-id="6a500-106">Developers should not use this type.</span></span> <span data-ttu-id="6a500-107">Os arquivos externos ainda podem ser indexados usando o [tipo externalItem.](externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="6a500-107">External files may still be indexed using the [externalItem](externalitem.md) type.</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a500-108">Um item indexado por meio de uma Pesquisa da Microsoft [conexão](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="6a500-108">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span> <span data-ttu-id="6a500-109">Esse tipo deriva do [tipo externalItem.](externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="6a500-109">This type derives from the [externalItem](externalitem.md) type.</span></span>

## <a name="methods"></a><span data-ttu-id="6a500-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="6a500-110">Methods</span></span>

| <span data-ttu-id="6a500-111">Método</span><span class="sxs-lookup"><span data-stu-id="6a500-111">Method</span></span>                                                        | <span data-ttu-id="6a500-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6a500-112">Return Type</span></span>  | <span data-ttu-id="6a500-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a500-113">Description</span></span> |
|:--------------------------------------------------------------|:-------------|:--|
| [<span data-ttu-id="6a500-114">Criar externalFile</span><span class="sxs-lookup"><span data-stu-id="6a500-114">Create externalFile</span></span>](../api/externalconnection-put-items.md) | <span data-ttu-id="6a500-115">externalFile</span><span class="sxs-lookup"><span data-stu-id="6a500-115">externalFile</span></span> | <span data-ttu-id="6a500-116">Crie um externalFile.</span><span class="sxs-lookup"><span data-stu-id="6a500-116">Create an externalFile.</span></span> |
| [<span data-ttu-id="6a500-117">Atualizar externalFile</span><span class="sxs-lookup"><span data-stu-id="6a500-117">Update externalFile</span></span>](../api/externalitem-update.md)          | <span data-ttu-id="6a500-118">externalFile</span><span class="sxs-lookup"><span data-stu-id="6a500-118">externalFile</span></span> | <span data-ttu-id="6a500-119">Atualize um externalFile.</span><span class="sxs-lookup"><span data-stu-id="6a500-119">Update an externalFile.</span></span> |
| [<span data-ttu-id="6a500-120">Delete</span><span class="sxs-lookup"><span data-stu-id="6a500-120">Delete</span></span>](../api/externalitem-delete.md)                       | <span data-ttu-id="6a500-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a500-121">None</span></span>         | <span data-ttu-id="6a500-122">Exclua um externalFile.</span><span class="sxs-lookup"><span data-stu-id="6a500-122">Delete an externalFile.</span></span> |

## <a name="properties"></a><span data-ttu-id="6a500-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a500-123">Properties</span></span>

| <span data-ttu-id="6a500-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a500-124">Property</span></span>         | <span data-ttu-id="6a500-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a500-125">Type</span></span>                     | <span data-ttu-id="6a500-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a500-126">Description</span></span>                    |
|:-----------------|:-------------------------|:-------------------------------|
| <span data-ttu-id="6a500-127">acl</span><span class="sxs-lookup"><span data-stu-id="6a500-127">acl</span></span>              | <span data-ttu-id="6a500-128">[Coleção acl](acl.md)</span><span class="sxs-lookup"><span data-stu-id="6a500-128">[acl](acl.md) collection</span></span> | <span data-ttu-id="6a500-129">Uma matriz de entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="6a500-129">An array of access control entries.</span></span> <span data-ttu-id="6a500-130">Cada entrada especifica o acesso concedido a um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="6a500-130">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="6a500-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a500-131">Required.</span></span> |
| <span data-ttu-id="6a500-132">content</span><span class="sxs-lookup"><span data-stu-id="6a500-132">content</span></span>          | <span data-ttu-id="6a500-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a500-133">String</span></span>                   | <span data-ttu-id="6a500-134">Uma representação em texto sem texto do conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="6a500-134">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="6a500-135">O texto nesta propriedade é indexado em texto completo.</span><span class="sxs-lookup"><span data-stu-id="6a500-135">The text in this property is full-text indexed.</span></span> <span data-ttu-id="6a500-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6a500-136">Optional.</span></span> |
| <span data-ttu-id="6a500-137">id</span><span class="sxs-lookup"><span data-stu-id="6a500-137">id</span></span>               | <span data-ttu-id="6a500-138">String</span><span class="sxs-lookup"><span data-stu-id="6a500-138">String</span></span>                   | <span data-ttu-id="6a500-139">ID exclusiva fornecida pelo desenvolvedor do item dentro do [externalConnection](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="6a500-139">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="6a500-140">Deve ser alfanumérico e um máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="6a500-140">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="6a500-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a500-141">Required.</span></span> |
| <span data-ttu-id="6a500-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="6a500-142">createdBy</span></span>        | <span data-ttu-id="6a500-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a500-143">String</span></span>                   | <span data-ttu-id="6a500-144">O nome do usuário que criou o arquivo.</span><span class="sxs-lookup"><span data-stu-id="6a500-144">The name of the user that created the file.</span></span> |
| <span data-ttu-id="6a500-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a500-145">createdDateTime</span></span>  | <span data-ttu-id="6a500-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a500-146">DateTimeOffset</span></span>           | <span data-ttu-id="6a500-147">A data e a hora em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="6a500-147">The date and time that the file was created.</span></span> <span data-ttu-id="6a500-148">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="6a500-148">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6a500-149">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="6a500-149">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span> |
| <span data-ttu-id="6a500-150">extension</span><span class="sxs-lookup"><span data-stu-id="6a500-150">extension</span></span>        | <span data-ttu-id="6a500-151">String</span><span class="sxs-lookup"><span data-stu-id="6a500-151">String</span></span>                   | <span data-ttu-id="6a500-152">A extensão de arquivo.</span><span class="sxs-lookup"><span data-stu-id="6a500-152">The file extension.</span></span>            |
| <span data-ttu-id="6a500-153">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6a500-153">lastModifiedBy</span></span>   | <span data-ttu-id="6a500-154">String</span><span class="sxs-lookup"><span data-stu-id="6a500-154">String</span></span>                   | <span data-ttu-id="6a500-155">O nome do usuário que modificou o arquivo pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6a500-155">The name of the user that last modified the file.</span></span> |
| <span data-ttu-id="6a500-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a500-156">modifiedDateTime</span></span> | <span data-ttu-id="6a500-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a500-157">DateTimeOffset</span></span>           | <span data-ttu-id="6a500-158">A data e a hora em que o arquivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6a500-158">The date and time that the file was last modified.</span></span> <span data-ttu-id="6a500-159">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="6a500-159">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6a500-160">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="6a500-160">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span> |
| <span data-ttu-id="6a500-161">nome</span><span class="sxs-lookup"><span data-stu-id="6a500-161">name</span></span>             | <span data-ttu-id="6a500-162">String</span><span class="sxs-lookup"><span data-stu-id="6a500-162">String</span></span>                   | <span data-ttu-id="6a500-163">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="6a500-163">The file name.</span></span> <span data-ttu-id="6a500-164">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a500-164">Required.</span></span>       |
| <span data-ttu-id="6a500-165">size</span><span class="sxs-lookup"><span data-stu-id="6a500-165">size</span></span>             | <span data-ttu-id="6a500-166">Int64</span><span class="sxs-lookup"><span data-stu-id="6a500-166">Int64</span></span>                    | <span data-ttu-id="6a500-167">O tamanho do arquivo em bytes.</span><span class="sxs-lookup"><span data-stu-id="6a500-167">The size of the file in bytes.</span></span> |
| <span data-ttu-id="6a500-168">title</span><span class="sxs-lookup"><span data-stu-id="6a500-168">title</span></span>            | <span data-ttu-id="6a500-169">String</span><span class="sxs-lookup"><span data-stu-id="6a500-169">String</span></span>                   | <span data-ttu-id="6a500-170">O título do arquivo.</span><span class="sxs-lookup"><span data-stu-id="6a500-170">The title of the file.</span></span>         |
| <span data-ttu-id="6a500-171">url</span><span class="sxs-lookup"><span data-stu-id="6a500-171">url</span></span>              | <span data-ttu-id="6a500-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a500-172">String</span></span>                   | <span data-ttu-id="6a500-173">A URL para acessar o arquivo.</span><span class="sxs-lookup"><span data-stu-id="6a500-173">The URL to access the file.</span></span> <span data-ttu-id="6a500-174">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a500-174">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6a500-175">Relações</span><span class="sxs-lookup"><span data-stu-id="6a500-175">Relationships</span></span>

<span data-ttu-id="6a500-176">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a500-176">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a500-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a500-177">JSON representation</span></span>

<span data-ttu-id="6a500-178">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a500-178">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalFile",
  "baseType": "microsoft.graph.externalItem"
}-->

```json
{
  "acl": [{"@odata.type": "microsoft.graph.acl"}],
  "content": "String",
  "id": "String (identifier)",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "extension": "String",
  "lastModifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "name": "String",
  "size": 1024,
  "title": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


