---
title: tipo de recurso externalfile
description: Um arquivo indexado por meio de uma conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8a4f4e9bb9a782e71dd0c2f349baaacc5b61f480
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892594"
---
# <a name="externalfile-resource-type"></a><span data-ttu-id="7235e-103">tipo de recurso externalfile</span><span class="sxs-lookup"><span data-stu-id="7235e-103">externalFile resource type</span></span>

<span data-ttu-id="7235e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7235e-104">Namespace: microsoft.graph</span></span>

> [!CAUTION]
> <span data-ttu-id="7235e-105">O `externalFile` tipo foi preterido.</span><span class="sxs-lookup"><span data-stu-id="7235e-105">The `externalFile` type has been deprecated.</span></span> <span data-ttu-id="7235e-106">Os desenvolvedores não devem usar esse tipo.</span><span class="sxs-lookup"><span data-stu-id="7235e-106">Developers should not use this type.</span></span> <span data-ttu-id="7235e-107">Arquivos externos ainda podem ser indexados usando o tipo [externalItem](externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="7235e-107">External files may still be indexed using the [externalItem](externalitem.md) type.</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7235e-108">Um item indexado por meio de uma [conexão](externalconnection.md)de pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7235e-108">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span> <span data-ttu-id="7235e-109">Esse tipo deriva do tipo [externalItem](externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="7235e-109">This type derives from the [externalItem](externalitem.md) type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="7235e-110">Methods</span><span class="sxs-lookup"><span data-stu-id="7235e-110">Methods</span></span>

| <span data-ttu-id="7235e-111">Método</span><span class="sxs-lookup"><span data-stu-id="7235e-111">Method</span></span>                                                        | <span data-ttu-id="7235e-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7235e-112">Return Type</span></span>  | <span data-ttu-id="7235e-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="7235e-113">Description</span></span> |
|:--------------------------------------------------------------|:-------------|:--|
| [<span data-ttu-id="7235e-114">Criar externalfile</span><span class="sxs-lookup"><span data-stu-id="7235e-114">Create externalFile</span></span>](../api/externalconnection-put-items.md) | <span data-ttu-id="7235e-115">externalFile</span><span class="sxs-lookup"><span data-stu-id="7235e-115">externalFile</span></span> | <span data-ttu-id="7235e-116">Criar um externalfile.</span><span class="sxs-lookup"><span data-stu-id="7235e-116">Create an externalFile.</span></span> |
| [<span data-ttu-id="7235e-117">Atualizar externalfile</span><span class="sxs-lookup"><span data-stu-id="7235e-117">Update externalFile</span></span>](../api/externalitem-update.md)          | <span data-ttu-id="7235e-118">externalFile</span><span class="sxs-lookup"><span data-stu-id="7235e-118">externalFile</span></span> | <span data-ttu-id="7235e-119">Atualize um externalfile.</span><span class="sxs-lookup"><span data-stu-id="7235e-119">Update an externalFile.</span></span> |
| [<span data-ttu-id="7235e-120">Delete</span><span class="sxs-lookup"><span data-stu-id="7235e-120">Delete</span></span>](../api/externalitem-delete.md)                       | <span data-ttu-id="7235e-121">None</span><span class="sxs-lookup"><span data-stu-id="7235e-121">None</span></span>         | <span data-ttu-id="7235e-122">Excluir um externalfile.</span><span class="sxs-lookup"><span data-stu-id="7235e-122">Delete an externalFile.</span></span> |

## <a name="properties"></a><span data-ttu-id="7235e-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7235e-123">Properties</span></span>

| <span data-ttu-id="7235e-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7235e-124">Property</span></span>         | <span data-ttu-id="7235e-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="7235e-125">Type</span></span>                     | <span data-ttu-id="7235e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="7235e-126">Description</span></span>                    |
|:-----------------|:-------------------------|:-------------------------------|
| <span data-ttu-id="7235e-127">ACL</span><span class="sxs-lookup"><span data-stu-id="7235e-127">acl</span></span>              | <span data-ttu-id="7235e-128">coleção [ACL](acl.md)</span><span class="sxs-lookup"><span data-stu-id="7235e-128">[acl](acl.md) collection</span></span> | <span data-ttu-id="7235e-129">Uma matriz de entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="7235e-129">An array of access control entries.</span></span> <span data-ttu-id="7235e-130">Cada entrada especifica o acesso concedido a um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="7235e-130">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="7235e-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7235e-131">Required.</span></span> |
| <span data-ttu-id="7235e-132">content</span><span class="sxs-lookup"><span data-stu-id="7235e-132">content</span></span>          | <span data-ttu-id="7235e-133">String</span><span class="sxs-lookup"><span data-stu-id="7235e-133">String</span></span>                   | <span data-ttu-id="7235e-134">Uma representação de texto simples do conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="7235e-134">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="7235e-135">O texto nessa propriedade é indexado de texto completo.</span><span class="sxs-lookup"><span data-stu-id="7235e-135">The text in this property is full-text indexed.</span></span> <span data-ttu-id="7235e-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7235e-136">Optional.</span></span> |
| <span data-ttu-id="7235e-137">id</span><span class="sxs-lookup"><span data-stu-id="7235e-137">id</span></span>               | <span data-ttu-id="7235e-138">String</span><span class="sxs-lookup"><span data-stu-id="7235e-138">String</span></span>                   | <span data-ttu-id="7235e-139">ID exclusiva fornecida pelo desenvolvedor do item dentro do [externalConnection](externalconnection.md)que contém o.</span><span class="sxs-lookup"><span data-stu-id="7235e-139">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="7235e-140">Deve ser alfanumérico e um máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="7235e-140">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="7235e-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7235e-141">Required.</span></span> |
| <span data-ttu-id="7235e-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="7235e-142">createdBy</span></span>        | <span data-ttu-id="7235e-143">String</span><span class="sxs-lookup"><span data-stu-id="7235e-143">String</span></span>                   | <span data-ttu-id="7235e-144">O nome do usuário que criou o arquivo.</span><span class="sxs-lookup"><span data-stu-id="7235e-144">The name of the user that created the file.</span></span> |
| <span data-ttu-id="7235e-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7235e-145">createdDateTime</span></span>  | <span data-ttu-id="7235e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7235e-146">DateTimeOffset</span></span>           | <span data-ttu-id="7235e-147">A data e hora em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="7235e-147">The date and time that the file was created.</span></span> <span data-ttu-id="7235e-148">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7235e-148">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7235e-149">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7235e-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="7235e-150">extensões</span><span class="sxs-lookup"><span data-stu-id="7235e-150">extension</span></span>        | <span data-ttu-id="7235e-151">String</span><span class="sxs-lookup"><span data-stu-id="7235e-151">String</span></span>                   | <span data-ttu-id="7235e-152">A extensão de arquivo.</span><span class="sxs-lookup"><span data-stu-id="7235e-152">The file extension.</span></span>            |
| <span data-ttu-id="7235e-153">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="7235e-153">lastModifiedBy</span></span>   | <span data-ttu-id="7235e-154">String</span><span class="sxs-lookup"><span data-stu-id="7235e-154">String</span></span>                   | <span data-ttu-id="7235e-155">O nome do usuário que modificou o arquivo pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7235e-155">The name of the user that last modified the file.</span></span> |
| <span data-ttu-id="7235e-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7235e-156">modifiedDateTime</span></span> | <span data-ttu-id="7235e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7235e-157">DateTimeOffset</span></span>           | <span data-ttu-id="7235e-158">A data e hora em que o arquivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7235e-158">The date and time that the file was last modified.</span></span> <span data-ttu-id="7235e-159">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7235e-159">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7235e-160">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7235e-160">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="7235e-161">nome</span><span class="sxs-lookup"><span data-stu-id="7235e-161">name</span></span>             | <span data-ttu-id="7235e-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7235e-162">String</span></span>                   | <span data-ttu-id="7235e-163">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="7235e-163">The file name.</span></span> <span data-ttu-id="7235e-164">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7235e-164">Required.</span></span>       |
| <span data-ttu-id="7235e-165">size</span><span class="sxs-lookup"><span data-stu-id="7235e-165">size</span></span>             | <span data-ttu-id="7235e-166">Int64</span><span class="sxs-lookup"><span data-stu-id="7235e-166">Int64</span></span>                    | <span data-ttu-id="7235e-167">O tamanho do arquivo em bytes.</span><span class="sxs-lookup"><span data-stu-id="7235e-167">The size of the file in bytes.</span></span> |
| <span data-ttu-id="7235e-168">title</span><span class="sxs-lookup"><span data-stu-id="7235e-168">title</span></span>            | <span data-ttu-id="7235e-169">String</span><span class="sxs-lookup"><span data-stu-id="7235e-169">String</span></span>                   | <span data-ttu-id="7235e-170">O título do arquivo.</span><span class="sxs-lookup"><span data-stu-id="7235e-170">The title of the file.</span></span>         |
| <span data-ttu-id="7235e-171">url</span><span class="sxs-lookup"><span data-stu-id="7235e-171">url</span></span>              | <span data-ttu-id="7235e-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7235e-172">String</span></span>                   | <span data-ttu-id="7235e-173">A URL para acessar o arquivo.</span><span class="sxs-lookup"><span data-stu-id="7235e-173">The URL to access the file.</span></span> <span data-ttu-id="7235e-174">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7235e-174">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7235e-175">Relações</span><span class="sxs-lookup"><span data-stu-id="7235e-175">Relationships</span></span>

<span data-ttu-id="7235e-176">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7235e-176">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7235e-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7235e-177">JSON representation</span></span>

<span data-ttu-id="7235e-178">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7235e-178">The following is a JSON representation of the resource.</span></span>

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
