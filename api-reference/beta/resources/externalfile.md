---
title: tipo de recurso externalfile
description: Um arquivo indexado por meio de uma conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 90faf3b10d09e84c9c0571d01fc242464888ff1e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071235"
---
# <a name="externalfile-resource-type"></a><span data-ttu-id="90abf-103">tipo de recurso externalfile</span><span class="sxs-lookup"><span data-stu-id="90abf-103">externalFile resource type</span></span>

<span data-ttu-id="90abf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90abf-104">Namespace: microsoft.graph</span></span>

> [!CAUTION]
> <span data-ttu-id="90abf-105">O `externalFile` tipo foi preterido.</span><span class="sxs-lookup"><span data-stu-id="90abf-105">The `externalFile` type has been deprecated.</span></span> <span data-ttu-id="90abf-106">Os desenvolvedores não devem usar esse tipo.</span><span class="sxs-lookup"><span data-stu-id="90abf-106">Developers should not use this type.</span></span> <span data-ttu-id="90abf-107">Arquivos externos ainda podem ser indexados usando o tipo [externalItem](externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="90abf-107">External files may still be indexed using the [externalItem](externalitem.md) type.</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90abf-108">Um item indexado por meio de uma [conexão](externalconnection.md)de pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="90abf-108">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span> <span data-ttu-id="90abf-109">Esse tipo deriva do tipo [externalItem](externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="90abf-109">This type derives from the [externalItem](externalitem.md) type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="90abf-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="90abf-110">Methods</span></span>

| <span data-ttu-id="90abf-111">Método</span><span class="sxs-lookup"><span data-stu-id="90abf-111">Method</span></span>                                                        | <span data-ttu-id="90abf-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="90abf-112">Return Type</span></span>  | <span data-ttu-id="90abf-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="90abf-113">Description</span></span> |
|:--------------------------------------------------------------|:-------------|:--|
| [<span data-ttu-id="90abf-114">Criar externalfile</span><span class="sxs-lookup"><span data-stu-id="90abf-114">Create externalFile</span></span>](../api/externalconnection-put-items.md) | <span data-ttu-id="90abf-115">externalFile</span><span class="sxs-lookup"><span data-stu-id="90abf-115">externalFile</span></span> | <span data-ttu-id="90abf-116">Criar um externalfile.</span><span class="sxs-lookup"><span data-stu-id="90abf-116">Create an externalFile.</span></span> |
| [<span data-ttu-id="90abf-117">Atualizar externalfile</span><span class="sxs-lookup"><span data-stu-id="90abf-117">Update externalFile</span></span>](../api/externalitem-update.md)          | <span data-ttu-id="90abf-118">externalFile</span><span class="sxs-lookup"><span data-stu-id="90abf-118">externalFile</span></span> | <span data-ttu-id="90abf-119">Atualize um externalfile.</span><span class="sxs-lookup"><span data-stu-id="90abf-119">Update an externalFile.</span></span> |
| [<span data-ttu-id="90abf-120">Delete</span><span class="sxs-lookup"><span data-stu-id="90abf-120">Delete</span></span>](../api/externalitem-delete.md)                       | <span data-ttu-id="90abf-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90abf-121">None</span></span>         | <span data-ttu-id="90abf-122">Excluir um externalfile.</span><span class="sxs-lookup"><span data-stu-id="90abf-122">Delete an externalFile.</span></span> |

## <a name="properties"></a><span data-ttu-id="90abf-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="90abf-123">Properties</span></span>

| <span data-ttu-id="90abf-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90abf-124">Property</span></span>         | <span data-ttu-id="90abf-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="90abf-125">Type</span></span>                     | <span data-ttu-id="90abf-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="90abf-126">Description</span></span>                    |
|:-----------------|:-------------------------|:-------------------------------|
| <span data-ttu-id="90abf-127">ACL</span><span class="sxs-lookup"><span data-stu-id="90abf-127">acl</span></span>              | <span data-ttu-id="90abf-128">coleção [ACL](acl.md)</span><span class="sxs-lookup"><span data-stu-id="90abf-128">[acl](acl.md) collection</span></span> | <span data-ttu-id="90abf-129">Uma matriz de entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="90abf-129">An array of access control entries.</span></span> <span data-ttu-id="90abf-130">Cada entrada especifica o acesso concedido a um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="90abf-130">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="90abf-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90abf-131">Required.</span></span> |
| <span data-ttu-id="90abf-132">content</span><span class="sxs-lookup"><span data-stu-id="90abf-132">content</span></span>          | <span data-ttu-id="90abf-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90abf-133">String</span></span>                   | <span data-ttu-id="90abf-134">Uma representação de texto simples do conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="90abf-134">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="90abf-135">O texto nessa propriedade é indexado de texto completo.</span><span class="sxs-lookup"><span data-stu-id="90abf-135">The text in this property is full-text indexed.</span></span> <span data-ttu-id="90abf-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="90abf-136">Optional.</span></span> |
| <span data-ttu-id="90abf-137">id</span><span class="sxs-lookup"><span data-stu-id="90abf-137">id</span></span>               | <span data-ttu-id="90abf-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90abf-138">String</span></span>                   | <span data-ttu-id="90abf-139">ID exclusiva fornecida pelo desenvolvedor do item dentro do [externalConnection](externalconnection.md)que contém o.</span><span class="sxs-lookup"><span data-stu-id="90abf-139">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="90abf-140">Deve ser alfanumérico e um máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="90abf-140">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="90abf-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90abf-141">Required.</span></span> |
| <span data-ttu-id="90abf-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="90abf-142">createdBy</span></span>        | <span data-ttu-id="90abf-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90abf-143">String</span></span>                   | <span data-ttu-id="90abf-144">O nome do usuário que criou o arquivo.</span><span class="sxs-lookup"><span data-stu-id="90abf-144">The name of the user that created the file.</span></span> |
| <span data-ttu-id="90abf-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90abf-145">createdDateTime</span></span>  | <span data-ttu-id="90abf-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90abf-146">DateTimeOffset</span></span>           | <span data-ttu-id="90abf-147">A data e hora em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="90abf-147">The date and time that the file was created.</span></span> <span data-ttu-id="90abf-148">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="90abf-148">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="90abf-149">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="90abf-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="90abf-150">extensões</span><span class="sxs-lookup"><span data-stu-id="90abf-150">extension</span></span>        | <span data-ttu-id="90abf-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90abf-151">String</span></span>                   | <span data-ttu-id="90abf-152">A extensão de arquivo.</span><span class="sxs-lookup"><span data-stu-id="90abf-152">The file extension.</span></span>            |
| <span data-ttu-id="90abf-153">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="90abf-153">lastModifiedBy</span></span>   | <span data-ttu-id="90abf-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90abf-154">String</span></span>                   | <span data-ttu-id="90abf-155">O nome do usuário que modificou o arquivo pela última vez.</span><span class="sxs-lookup"><span data-stu-id="90abf-155">The name of the user that last modified the file.</span></span> |
| <span data-ttu-id="90abf-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90abf-156">modifiedDateTime</span></span> | <span data-ttu-id="90abf-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90abf-157">DateTimeOffset</span></span>           | <span data-ttu-id="90abf-158">A data e hora em que o arquivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="90abf-158">The date and time that the file was last modified.</span></span> <span data-ttu-id="90abf-159">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="90abf-159">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="90abf-160">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="90abf-160">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="90abf-161">name</span><span class="sxs-lookup"><span data-stu-id="90abf-161">name</span></span>             | <span data-ttu-id="90abf-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90abf-162">String</span></span>                   | <span data-ttu-id="90abf-163">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="90abf-163">The file name.</span></span> <span data-ttu-id="90abf-164">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90abf-164">Required.</span></span>       |
| <span data-ttu-id="90abf-165">size</span><span class="sxs-lookup"><span data-stu-id="90abf-165">size</span></span>             | <span data-ttu-id="90abf-166">Int64</span><span class="sxs-lookup"><span data-stu-id="90abf-166">Int64</span></span>                    | <span data-ttu-id="90abf-167">O tamanho do arquivo em bytes.</span><span class="sxs-lookup"><span data-stu-id="90abf-167">The size of the file in bytes.</span></span> |
| <span data-ttu-id="90abf-168">title</span><span class="sxs-lookup"><span data-stu-id="90abf-168">title</span></span>            | <span data-ttu-id="90abf-169">String</span><span class="sxs-lookup"><span data-stu-id="90abf-169">String</span></span>                   | <span data-ttu-id="90abf-170">O título do arquivo.</span><span class="sxs-lookup"><span data-stu-id="90abf-170">The title of the file.</span></span>         |
| <span data-ttu-id="90abf-171">url</span><span class="sxs-lookup"><span data-stu-id="90abf-171">url</span></span>              | <span data-ttu-id="90abf-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90abf-172">String</span></span>                   | <span data-ttu-id="90abf-173">A URL para acessar o arquivo.</span><span class="sxs-lookup"><span data-stu-id="90abf-173">The URL to access the file.</span></span> <span data-ttu-id="90abf-174">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90abf-174">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="90abf-175">Relações</span><span class="sxs-lookup"><span data-stu-id="90abf-175">Relationships</span></span>

<span data-ttu-id="90abf-176">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90abf-176">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90abf-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="90abf-177">JSON representation</span></span>

<span data-ttu-id="90abf-178">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="90abf-178">The following is a JSON representation of the resource.</span></span>

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


