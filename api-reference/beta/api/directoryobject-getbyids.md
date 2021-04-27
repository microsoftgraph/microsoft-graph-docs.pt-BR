---
title: 'directoryObject: getByIds'
description: 'Retorna os objetos de diretório especificados em uma lista de IDs. '
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 72e580e3ad36540ae40311358bf065d67a74f59a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046857"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="f23d0-103">Obter objetos directory a partir de uma lista de ids</span><span class="sxs-lookup"><span data-stu-id="f23d0-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="f23d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f23d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f23d0-105">Retorne os objetos de diretório especificados em uma lista de IDs.</span><span class="sxs-lookup"><span data-stu-id="f23d0-105">Return the directory objects specified in a list of IDs.</span></span>

<span data-ttu-id="f23d0-106">Alguns usos comuns dessa função são:</span><span class="sxs-lookup"><span data-stu-id="f23d0-106">Some common uses for this function are to:</span></span>

* <span data-ttu-id="f23d0-107">Resolva as IDs retornadas por funções (que retornam coleções de IDs) como [getMemberObjects](./directoryobject-getmemberobjects.md) ou [getMemberGroups](./directoryobject-getmembergroups.md) para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="f23d0-107">Resolve IDs returned by functions (that return collections of IDs) such as [getMemberObjects](./directoryobject-getmemberobjects.md) or [getMemberGroups](./directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="f23d0-108">Resolva IDs que persistem em um repositório externo pelo aplicativo para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="f23d0-108">Resolve IDs persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f23d0-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f23d0-109">Permissions</span></span>

<span data-ttu-id="f23d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f23d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f23d0-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f23d0-112">Permission type</span></span>      | <span data-ttu-id="f23d0-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f23d0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f23d0-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f23d0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f23d0-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f23d0-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="f23d0-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f23d0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f23d0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f23d0-117">Not supported.</span></span>    |
|<span data-ttu-id="f23d0-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f23d0-118">Application</span></span> | <span data-ttu-id="f23d0-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f23d0-119">Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="f23d0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f23d0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="f23d0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f23d0-121">Request headers</span></span>

| <span data-ttu-id="f23d0-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f23d0-122">Name</span></span>       | <span data-ttu-id="f23d0-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f23d0-123">Type</span></span> | <span data-ttu-id="f23d0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f23d0-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f23d0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f23d0-125">Authorization</span></span>  | <span data-ttu-id="f23d0-126">string</span><span class="sxs-lookup"><span data-stu-id="f23d0-126">string</span></span>  | <span data-ttu-id="f23d0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f23d0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f23d0-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="f23d0-129">Content-type</span></span>  | <span data-ttu-id="f23d0-130">string</span><span class="sxs-lookup"><span data-stu-id="f23d0-130">string</span></span> | <span data-ttu-id="f23d0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f23d0-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f23d0-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f23d0-133">Request body</span></span>

<span data-ttu-id="f23d0-134">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f23d0-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f23d0-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f23d0-135">Parameter</span></span>   | <span data-ttu-id="f23d0-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="f23d0-136">Type</span></span> |<span data-ttu-id="f23d0-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="f23d0-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f23d0-138">ids</span><span class="sxs-lookup"><span data-stu-id="f23d0-138">ids</span></span>|<span data-ttu-id="f23d0-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f23d0-139">String collection</span></span>| <span data-ttu-id="f23d0-140">Uma coleção de IDs para a qual retornar objetos.</span><span class="sxs-lookup"><span data-stu-id="f23d0-140">A collection of IDs for which to return objects.</span></span> <span data-ttu-id="f23d0-141">As IDs são GUIDs, representadas como cadeias de caracteres.</span><span class="sxs-lookup"><span data-stu-id="f23d0-141">The IDs are GUIDs, represented as strings.</span></span> <span data-ttu-id="f23d0-142">Você pode especificar até 1000 IDs.</span><span class="sxs-lookup"><span data-stu-id="f23d0-142">You can specify up to 1000 IDs.</span></span> |
|<span data-ttu-id="f23d0-143">tipos</span><span class="sxs-lookup"><span data-stu-id="f23d0-143">types</span></span>|<span data-ttu-id="f23d0-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f23d0-144">String collection</span></span>| <span data-ttu-id="f23d0-145">Uma coleção de tipos de recursos que especifica o conjunto de coleções de recursos para pesquisar.</span><span class="sxs-lookup"><span data-stu-id="f23d0-145">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="f23d0-146">Se não estiver especificado, o padrão será [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), que contém todos os tipos de recursos definidos no diretório.</span><span class="sxs-lookup"><span data-stu-id="f23d0-146">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="f23d0-147">Qualquer objeto deriva do [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) pode ser especificado na coleção. Por exemplo: [usuário](/graph/api/resources/user?view=graph-rest-beta), [grupo](/graph/api/resources/group?view=graph-rest-beta), [dispositivo](/graph/api/resources/device?view=graph-rest-beta) e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="f23d0-147">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta), [device](/graph/api/resources/device?view=graph-rest-beta), and so on.</span></span> <span data-ttu-id="f23d0-148">Para procurar referências para uma organização parceira do [Provedor de soluções de nuvem](https://partner.microsoft.com/cloud-solution-provider) especifique [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="f23d0-148">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span></span> <span data-ttu-id="f23d0-149">Se não for especificado, o padrão é [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta),  que contém todos os tipos de recursos definidos no diretório, exceto referências a uma organização parceira do [Provedor de soluções de nuvem](https://partner.microsoft.com/cloud-solution-provider).</span><span class="sxs-lookup"><span data-stu-id="f23d0-149">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="f23d0-150">Os valores não diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="f23d0-150">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="f23d0-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="f23d0-151">Response</span></span>

<span data-ttu-id="f23d0-152">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f23d0-152">If successful, this method returns a `200 OK` response code and a string collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f23d0-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f23d0-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="f23d0-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f23d0-154">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f23d0-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="f23d0-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f23d0-156">C#</span><span class="sxs-lookup"><span data-stu-id="f23d0-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f23d0-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f23d0-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f23d0-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f23d0-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f23d0-159">Java</span><span class="sxs-lookup"><span data-stu-id="f23d0-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getbyids-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f23d0-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="f23d0-160">Response</span></span>

><span data-ttu-id="f23d0-161">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f23d0-161">**Note:** The response object shown here might be shortened for readability.</span></span>

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
