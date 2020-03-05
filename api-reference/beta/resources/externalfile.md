---
title: tipo de recurso externalfile
description: Um arquivo indexado por meio de uma conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 91de559bd365b9d6141e10a82af9ee06593f08ef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498774"
---
# <a name="externalfile-resource-type"></a><span data-ttu-id="8826c-103">tipo de recurso externalfile</span><span class="sxs-lookup"><span data-stu-id="8826c-103">externalFile resource type</span></span>

<span data-ttu-id="8826c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8826c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8826c-105">Um item indexado por meio de uma [conexão](externalconnection.md)de pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8826c-105">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span> <span data-ttu-id="8826c-106">Esse tipo deriva do tipo [externalItem](externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="8826c-106">This type derives from the [externalItem](externalitem.md) type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="8826c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="8826c-107">Methods</span></span>

| <span data-ttu-id="8826c-108">Método</span><span class="sxs-lookup"><span data-stu-id="8826c-108">Method</span></span>                                                        | <span data-ttu-id="8826c-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8826c-109">Return Type</span></span>  | <span data-ttu-id="8826c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8826c-110">Description</span></span> |
|:--------------------------------------------------------------|:-------------|:--|
| [<span data-ttu-id="8826c-111">Criar externalfile</span><span class="sxs-lookup"><span data-stu-id="8826c-111">Create externalFile</span></span>](../api/externalconnection-put-items.md) | <span data-ttu-id="8826c-112">externalFile</span><span class="sxs-lookup"><span data-stu-id="8826c-112">externalFile</span></span> | <span data-ttu-id="8826c-113">Criar um externalfile.</span><span class="sxs-lookup"><span data-stu-id="8826c-113">Create an externalFile.</span></span> |
| [<span data-ttu-id="8826c-114">Atualizar externalfile</span><span class="sxs-lookup"><span data-stu-id="8826c-114">Update externalFile</span></span>](../api/externalitem-update.md)          | <span data-ttu-id="8826c-115">externalFile</span><span class="sxs-lookup"><span data-stu-id="8826c-115">externalFile</span></span> | <span data-ttu-id="8826c-116">Atualize um externalfile.</span><span class="sxs-lookup"><span data-stu-id="8826c-116">Update an externalFile.</span></span> |
| [<span data-ttu-id="8826c-117">Delete</span><span class="sxs-lookup"><span data-stu-id="8826c-117">Delete</span></span>](../api/externalitem-delete.md)                       | <span data-ttu-id="8826c-118">None</span><span class="sxs-lookup"><span data-stu-id="8826c-118">None</span></span>         | <span data-ttu-id="8826c-119">Excluir um externalfile.</span><span class="sxs-lookup"><span data-stu-id="8826c-119">Delete an externalFile.</span></span> |

## <a name="properties"></a><span data-ttu-id="8826c-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8826c-120">Properties</span></span>

| <span data-ttu-id="8826c-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8826c-121">Property</span></span>         | <span data-ttu-id="8826c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="8826c-122">Type</span></span>                     | <span data-ttu-id="8826c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8826c-123">Description</span></span>                    |
|:-----------------|:-------------------------|:-------------------------------|
| <span data-ttu-id="8826c-124">ACL</span><span class="sxs-lookup"><span data-stu-id="8826c-124">acl</span></span>              | <span data-ttu-id="8826c-125">coleção [ACL](acl.md)</span><span class="sxs-lookup"><span data-stu-id="8826c-125">[acl](acl.md) collection</span></span> | <span data-ttu-id="8826c-126">Uma matriz de entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="8826c-126">An array of access control entries.</span></span> <span data-ttu-id="8826c-127">Cada entrada especifica o acesso concedido a um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="8826c-127">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="8826c-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8826c-128">Required.</span></span> |
| <span data-ttu-id="8826c-129">content</span><span class="sxs-lookup"><span data-stu-id="8826c-129">content</span></span>          | <span data-ttu-id="8826c-130">String</span><span class="sxs-lookup"><span data-stu-id="8826c-130">String</span></span>                   | <span data-ttu-id="8826c-131">Uma representação de texto simples do conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="8826c-131">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="8826c-132">O texto nessa propriedade é indexado de texto completo.</span><span class="sxs-lookup"><span data-stu-id="8826c-132">The text in this property is full-text indexed.</span></span> <span data-ttu-id="8826c-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8826c-133">Optional.</span></span> |
| <span data-ttu-id="8826c-134">id</span><span class="sxs-lookup"><span data-stu-id="8826c-134">id</span></span>               | <span data-ttu-id="8826c-135">String</span><span class="sxs-lookup"><span data-stu-id="8826c-135">String</span></span>                   | <span data-ttu-id="8826c-136">ID exclusiva fornecida pelo desenvolvedor do item dentro do [externalConnection](externalconnection.md)que contém o.</span><span class="sxs-lookup"><span data-stu-id="8826c-136">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="8826c-137">Deve ser alfanumérico e um máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="8826c-137">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="8826c-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8826c-138">Required.</span></span> |
| <span data-ttu-id="8826c-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="8826c-139">createdBy</span></span>        | <span data-ttu-id="8826c-140">String</span><span class="sxs-lookup"><span data-stu-id="8826c-140">String</span></span>                   | <span data-ttu-id="8826c-141">O nome do usuário que criou o arquivo.</span><span class="sxs-lookup"><span data-stu-id="8826c-141">The name of the user that created the file.</span></span> |
| <span data-ttu-id="8826c-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8826c-142">createdDateTime</span></span>  | <span data-ttu-id="8826c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8826c-143">DateTimeOffset</span></span>           | <span data-ttu-id="8826c-144">A data e hora em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="8826c-144">The date and time that the file was created.</span></span> <span data-ttu-id="8826c-145">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8826c-145">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8826c-146">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8826c-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="8826c-147">extensões</span><span class="sxs-lookup"><span data-stu-id="8826c-147">extension</span></span>        | <span data-ttu-id="8826c-148">String</span><span class="sxs-lookup"><span data-stu-id="8826c-148">String</span></span>                   | <span data-ttu-id="8826c-149">A extensão de arquivo.</span><span class="sxs-lookup"><span data-stu-id="8826c-149">The file extension.</span></span>            |
| <span data-ttu-id="8826c-150">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8826c-150">lastModifiedBy</span></span>   | <span data-ttu-id="8826c-151">String</span><span class="sxs-lookup"><span data-stu-id="8826c-151">String</span></span>                   | <span data-ttu-id="8826c-152">O nome do usuário que modificou o arquivo pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8826c-152">The name of the user that last modified the file.</span></span> |
| <span data-ttu-id="8826c-153">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8826c-153">modifiedDateTime</span></span> | <span data-ttu-id="8826c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8826c-154">DateTimeOffset</span></span>           | <span data-ttu-id="8826c-155">A data e hora em que o arquivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8826c-155">The date and time that the file was last modified.</span></span> <span data-ttu-id="8826c-156">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8826c-156">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8826c-157">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8826c-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="8826c-158">nome</span><span class="sxs-lookup"><span data-stu-id="8826c-158">name</span></span>             | <span data-ttu-id="8826c-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8826c-159">String</span></span>                   | <span data-ttu-id="8826c-160">O nome do arquivo.</span><span class="sxs-lookup"><span data-stu-id="8826c-160">The file name.</span></span> <span data-ttu-id="8826c-161">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8826c-161">Required.</span></span>       |
| <span data-ttu-id="8826c-162">size</span><span class="sxs-lookup"><span data-stu-id="8826c-162">size</span></span>             | <span data-ttu-id="8826c-163">Int64</span><span class="sxs-lookup"><span data-stu-id="8826c-163">Int64</span></span>                    | <span data-ttu-id="8826c-164">O tamanho do arquivo em bytes.</span><span class="sxs-lookup"><span data-stu-id="8826c-164">The size of the file in bytes.</span></span> |
| <span data-ttu-id="8826c-165">title</span><span class="sxs-lookup"><span data-stu-id="8826c-165">title</span></span>            | <span data-ttu-id="8826c-166">String</span><span class="sxs-lookup"><span data-stu-id="8826c-166">String</span></span>                   | <span data-ttu-id="8826c-167">O título do arquivo.</span><span class="sxs-lookup"><span data-stu-id="8826c-167">The title of the file.</span></span>         |
| <span data-ttu-id="8826c-168">url</span><span class="sxs-lookup"><span data-stu-id="8826c-168">url</span></span>              | <span data-ttu-id="8826c-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8826c-169">String</span></span>                   | <span data-ttu-id="8826c-170">A URL para acessar o arquivo.</span><span class="sxs-lookup"><span data-stu-id="8826c-170">The URL to access the file.</span></span> <span data-ttu-id="8826c-171">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8826c-171">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8826c-172">Relações</span><span class="sxs-lookup"><span data-stu-id="8826c-172">Relationships</span></span>

<span data-ttu-id="8826c-173">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8826c-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8826c-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8826c-174">JSON representation</span></span>

<span data-ttu-id="8826c-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8826c-175">The following is a JSON representation of the resource.</span></span>

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
