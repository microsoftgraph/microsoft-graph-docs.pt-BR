---
title: Obter objetos directory a partir de uma lista de ids
description: A opção selecionar não está disponível para todos os tipos de arquivo.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 093e39a6d70193c03d0b2ae9d91b61f6bdf5bbbb
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43180941"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="9bf3c-103">Obter objetos directory a partir de uma lista de ids</span><span class="sxs-lookup"><span data-stu-id="9bf3c-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="9bf3c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bf3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bf3c-p101">Retorna os objetos directory especificados a partir de uma lista de ids  OBSERVAÇÃO: Os objetos de diretório retornados são os objetos completos que contêm **todas** as propriedades. A opção `$select` não está disponível para todos os tipos de arquivo.</span><span class="sxs-lookup"><span data-stu-id="9bf3c-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="9bf3c-108">Alguns usos comuns dessa função são:</span><span class="sxs-lookup"><span data-stu-id="9bf3c-108">Some common uses for this function are to:</span></span>

* <span data-ttu-id="9bf3c-109">Resolver ids retornadas por funções (que retornam coleções de ids) como [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) ou [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta) para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="9bf3c-109">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) or [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta)  to their backing directory objects.</span></span>
* <span data-ttu-id="9bf3c-110">Resolver ids que persistem em um repositório externo pelo aplicativo para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="9bf3c-110">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9bf3c-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="9bf3c-111">Permissions</span></span>

<span data-ttu-id="9bf3c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bf3c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9bf3c-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bf3c-114">Permission type</span></span>      | <span data-ttu-id="9bf3c-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9bf3c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bf3c-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bf3c-116">Delegated (work or school account)</span></span> | <span data-ttu-id="9bf3c-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bf3c-117">Directory.Read.All</span></span>    |
|<span data-ttu-id="9bf3c-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bf3c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bf3c-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bf3c-119">Not supported.</span></span>    |
|<span data-ttu-id="9bf3c-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9bf3c-120">Application</span></span> | <span data-ttu-id="9bf3c-121">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bf3c-121">Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="9bf3c-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bf3c-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="9bf3c-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bf3c-123">Request headers</span></span>

| <span data-ttu-id="9bf3c-124">Nome</span><span class="sxs-lookup"><span data-stu-id="9bf3c-124">Name</span></span>       | <span data-ttu-id="9bf3c-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bf3c-125">Type</span></span> | <span data-ttu-id="9bf3c-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bf3c-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9bf3c-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bf3c-127">Authorization</span></span>  | <span data-ttu-id="9bf3c-128">string</span><span class="sxs-lookup"><span data-stu-id="9bf3c-128">string</span></span>  | <span data-ttu-id="9bf3c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bf3c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9bf3c-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9bf3c-131">Content-Type</span></span>  | <span data-ttu-id="9bf3c-132">application/json</span><span class="sxs-lookup"><span data-stu-id="9bf3c-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9bf3c-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9bf3c-133">Request body</span></span>

<span data-ttu-id="9bf3c-134">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9bf3c-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9bf3c-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9bf3c-135">Parameter</span></span>   | <span data-ttu-id="9bf3c-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bf3c-136">Type</span></span> |<span data-ttu-id="9bf3c-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bf3c-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9bf3c-138">ids</span><span class="sxs-lookup"><span data-stu-id="9bf3c-138">ids</span></span>|<span data-ttu-id="9bf3c-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bf3c-139">String collection</span></span>| <span data-ttu-id="9bf3c-p104">Uma coleção de ids para a qual retornar objetos. Você pode especificar até 1000 ids.</span><span class="sxs-lookup"><span data-stu-id="9bf3c-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="9bf3c-142">tipos</span><span class="sxs-lookup"><span data-stu-id="9bf3c-142">types</span></span>|<span data-ttu-id="9bf3c-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bf3c-143">String collection</span></span>| <span data-ttu-id="9bf3c-144">Uma coleção de tipos de recursos que especifica o conjunto de coleções de recursos para pesquisar.</span><span class="sxs-lookup"><span data-stu-id="9bf3c-144">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="9bf3c-145">Se não estiver especificado, o padrão será [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), que contém todos os tipos de recursos definidos no diretório.</span><span class="sxs-lookup"><span data-stu-id="9bf3c-145">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="9bf3c-146">Qualquer objeto deriva do [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) pode ser especificado na coleção. Por exemplo: [usuário](/graph/api/resources/user?view=graph-rest-beta), [grupo](/graph/api/resources/group?view=graph-rest-beta), [dispositivo](/graph/api/resources/device?view=graph-rest-beta) e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="9bf3c-146">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta), [device](/graph/api/resources/device?view=graph-rest-beta), and so on.</span></span> <span data-ttu-id="9bf3c-147">Para procurar referências para uma organização parceira do [Provedor de soluções de nuvem](https://partner.microsoft.com/en-us/cloud-solution-provider) especifique [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="9bf3c-147">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span></span> <span data-ttu-id="9bf3c-148">Se não for especificado, o padrão é [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta),  que contém todos os tipos de recursos definidos no diretório, exceto referências a uma organização parceira do [Provedor de soluções de nuvem](https://partner.microsoft.com/en-us/cloud-solution-provider).</span><span class="sxs-lookup"><span data-stu-id="9bf3c-148">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="9bf3c-149">Os valores não diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9bf3c-149">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="9bf3c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bf3c-150">Response</span></span>

<span data-ttu-id="9bf3c-151">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bf3c-151">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bf3c-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bf3c-152">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9bf3c-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bf3c-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9bf3c-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bf3c-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getByIds"
}-->

```http
POST https://graph.microsoft.com/beta/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893-8749-40a3-97b7-68513b600544","5d6059b6-368d-45f8-91e1-8e07d485f1d0"],
    "types":["user"]
}
```
# <a name="c"></a>[<span data-ttu-id="9bf3c-155">C#</span><span class="sxs-lookup"><span data-stu-id="9bf3c-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9bf3c-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bf3c-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9bf3c-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9bf3c-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9bf3c-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bf3c-158">Response</span></span>

<span data-ttu-id="9bf3c-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9bf3c-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
    "value": [
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Trevor Jones"
      },
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Billy Smith"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
