---
title: tipo de recurso externalfile
description: Um arquivo indexado por meio de uma conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c3e51c27985927f5ea71f8ca618c4055a609fc06
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703746"
---
# <a name="externalfile-resource-type"></a><span data-ttu-id="8d11b-103">tipo de recurso externalfile</span><span class="sxs-lookup"><span data-stu-id="8d11b-103">externalFile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d11b-104">Um item indexado por meio de uma [conexão](externalconnection.md)de pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8d11b-104">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span> <span data-ttu-id="8d11b-105">Esse tipo deriva do tipo [externalItem](externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="8d11b-105">This type derives from the [externalItem](externalitem.md) type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="8d11b-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8d11b-106">Methods</span></span>

| <span data-ttu-id="8d11b-107">Método</span><span class="sxs-lookup"><span data-stu-id="8d11b-107">Method</span></span>                                                        | <span data-ttu-id="8d11b-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8d11b-108">Return Type</span></span>  | <span data-ttu-id="8d11b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d11b-109">Description</span></span> |
|:--------------------------------------------------------------|:-------------|:--|
| [<span data-ttu-id="8d11b-110">Criar externalfile</span><span class="sxs-lookup"><span data-stu-id="8d11b-110">Create externalFile</span></span>](../api/externalconnection-put-items.md) | <span data-ttu-id="8d11b-111">externalFile</span><span class="sxs-lookup"><span data-stu-id="8d11b-111">externalFile</span></span> | <span data-ttu-id="8d11b-112">Criar um externalfile.</span><span class="sxs-lookup"><span data-stu-id="8d11b-112">Create an externalFile.</span></span> |
| [<span data-ttu-id="8d11b-113">Atualizar externalfile</span><span class="sxs-lookup"><span data-stu-id="8d11b-113">Update externalFile</span></span>](../api/externalitem-update.md)          | <span data-ttu-id="8d11b-114">externalFile</span><span class="sxs-lookup"><span data-stu-id="8d11b-114">externalFile</span></span> | <span data-ttu-id="8d11b-115">Atualize um externalfile.</span><span class="sxs-lookup"><span data-stu-id="8d11b-115">Update an externalFile.</span></span> |
| [<span data-ttu-id="8d11b-116">Excluir</span><span class="sxs-lookup"><span data-stu-id="8d11b-116">Delete</span></span>](../api/externalitem-delete.md)                       | <span data-ttu-id="8d11b-117">None</span><span class="sxs-lookup"><span data-stu-id="8d11b-117">None</span></span>         | <span data-ttu-id="8d11b-118">Excluir um externalfile.</span><span class="sxs-lookup"><span data-stu-id="8d11b-118">Delete an externalFile.</span></span> |

## <a name="properties"></a><span data-ttu-id="8d11b-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d11b-119">Properties</span></span>

| <span data-ttu-id="8d11b-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d11b-120">Property</span></span>         | <span data-ttu-id="8d11b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d11b-121">Type</span></span>                     | <span data-ttu-id="8d11b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d11b-122">Description</span></span>                    |
|:-----------------|:-------------------------|:-------------------------------|
| <span data-ttu-id="8d11b-123">ACL</span><span class="sxs-lookup"><span data-stu-id="8d11b-123">acl</span></span>              | <span data-ttu-id="8d11b-124">coleção [ACL](acl.md)</span><span class="sxs-lookup"><span data-stu-id="8d11b-124">[acl](acl.md) collection</span></span> | <span data-ttu-id="8d11b-125">Uma matriz de entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="8d11b-125">An array of access control entries.</span></span> <span data-ttu-id="8d11b-126">Cada entrada especifica o acesso concedido a um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="8d11b-126">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="8d11b-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d11b-127">Required.</span></span> |
| <span data-ttu-id="8d11b-128">content</span><span class="sxs-lookup"><span data-stu-id="8d11b-128">content</span></span>          | <span data-ttu-id="8d11b-129">String</span><span class="sxs-lookup"><span data-stu-id="8d11b-129">String</span></span>                   | <span data-ttu-id="8d11b-130">Uma representação de texto simples do conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="8d11b-130">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="8d11b-131">O texto nessa propriedade é indexado de texto completo.</span><span class="sxs-lookup"><span data-stu-id="8d11b-131">The text in this property is full-text indexed.</span></span> <span data-ttu-id="8d11b-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8d11b-132">Optional.</span></span> |
| <span data-ttu-id="8d11b-133">id</span><span class="sxs-lookup"><span data-stu-id="8d11b-133">id</span></span>               | <span data-ttu-id="8d11b-134">String</span><span class="sxs-lookup"><span data-stu-id="8d11b-134">String</span></span>                   | <span data-ttu-id="8d11b-135">ID exclusiva fornecida pelo desenvolvedor do item dentro do [externalConnection](externalconnection.md)que contém o.</span><span class="sxs-lookup"><span data-stu-id="8d11b-135">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="8d11b-136">Deve ser alfanumérico e um máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="8d11b-136">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="8d11b-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d11b-137">Required.</span></span> |
| <span data-ttu-id="8d11b-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="8d11b-138">createdBy</span></span>        | <span data-ttu-id="8d11b-139">String</span><span class="sxs-lookup"><span data-stu-id="8d11b-139">String</span></span>                   | <span data-ttu-id="8d11b-140">O nome do usuário que criou o arquivo.</span><span class="sxs-lookup"><span data-stu-id="8d11b-140">The name of the user that created the file.</span></span> |
| <span data-ttu-id="8d11b-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d11b-141">createdDateTime</span></span>  | <span data-ttu-id="8d11b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d11b-142">DateTimeOffset</span></span>           | <span data-ttu-id="8d11b-143">A data e hora em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="8d11b-143">The date and time that the file was created.</span></span> <span data-ttu-id="8d11b-144">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8d11b-144">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8d11b-145">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8d11b-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="8d11b-146">extensões</span><span class="sxs-lookup"><span data-stu-id="8d11b-146">extension</span></span>        | <span data-ttu-id="8d11b-147">String</span><span class="sxs-lookup"><span data-stu-id="8d11b-147">String</span></span>                   | <span data-ttu-id="8d11b-148">A extensão de arquivo.</span><span class="sxs-lookup"><span data-stu-id="8d11b-148">The file extension.</span></span>            |
| <span data-ttu-id="8d11b-149">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8d11b-149">lastModifiedBy</span></span>   | <span data-ttu-id="8d11b-150">String</span><span class="sxs-lookup"><span data-stu-id="8d11b-150">String</span></span>                   | <span data-ttu-id="8d11b-151">O nome do usuário que modificou o arquivo pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8d11b-151">The name of the user that last modified the file.</span></span> |
| <span data-ttu-id="8d11b-152">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d11b-152">modifiedDateTime</span></span> | <span data-ttu-id="8d11b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d11b-153">DateTimeOffset</span></span>           | <span data-ttu-id="8d11b-154">A data e hora em que o arquivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8d11b-154">The date and time that the file was last modified.</span></span> <span data-ttu-id="8d11b-155">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8d11b-155">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8d11b-156">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8d11b-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="8d11b-157">name</span><span class="sxs-lookup"><span data-stu-id="8d11b-157">name</span></span>             | <span data-ttu-id="8d11b-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d11b-158">String</span></span>                   | <span data-ttu-id="8d11b-159">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="8d11b-159">The file name.</span></span> <span data-ttu-id="8d11b-160">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d11b-160">Required.</span></span>       |
| <span data-ttu-id="8d11b-161">size</span><span class="sxs-lookup"><span data-stu-id="8d11b-161">size</span></span>             | <span data-ttu-id="8d11b-162">Int64</span><span class="sxs-lookup"><span data-stu-id="8d11b-162">Int64</span></span>                    | <span data-ttu-id="8d11b-163">O tamanho do arquivo em bytes.</span><span class="sxs-lookup"><span data-stu-id="8d11b-163">The size of the file in bytes.</span></span> |
| <span data-ttu-id="8d11b-164">title</span><span class="sxs-lookup"><span data-stu-id="8d11b-164">title</span></span>            | <span data-ttu-id="8d11b-165">String</span><span class="sxs-lookup"><span data-stu-id="8d11b-165">String</span></span>                   | <span data-ttu-id="8d11b-166">O título do arquivo.</span><span class="sxs-lookup"><span data-stu-id="8d11b-166">The title of the file.</span></span>         |
| <span data-ttu-id="8d11b-167">url</span><span class="sxs-lookup"><span data-stu-id="8d11b-167">url</span></span>              | <span data-ttu-id="8d11b-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d11b-168">String</span></span>                   | <span data-ttu-id="8d11b-169">A URL para acessar o arquivo.</span><span class="sxs-lookup"><span data-stu-id="8d11b-169">The URL to access the file.</span></span> <span data-ttu-id="8d11b-170">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d11b-170">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8d11b-171">Relações</span><span class="sxs-lookup"><span data-stu-id="8d11b-171">Relationships</span></span>

<span data-ttu-id="8d11b-172">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8d11b-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d11b-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d11b-173">JSON representation</span></span>

<span data-ttu-id="8d11b-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8d11b-174">The following is a JSON representation of the resource.</span></span>

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
