---
title: 'directoryObject: getByIds'
description: Retorna os objetos de diretório especificados em uma lista de IDs.
author: keylimesoda
localization_priority: Priority
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: bcd1e20de65f6ddefc08310572ff596865d438da
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051491"
---
# <a name="directoryobject-getbyids"></a><span data-ttu-id="5e828-103">directoryObject: getByIds</span><span class="sxs-lookup"><span data-stu-id="5e828-103">directoryObject: getByIds</span></span>

<span data-ttu-id="5e828-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e828-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5e828-105">Retorne os objetos de diretório especificados em uma lista de IDs.</span><span class="sxs-lookup"><span data-stu-id="5e828-105">Return the directory objects specified in a list of IDs.</span></span>

>[!NOTE]
><span data-ttu-id="5e828-106">Essa API tem um [problema conhecido](/graph/known-issues#incomplete-objects-when-using-getbyids-request).</span><span class="sxs-lookup"><span data-stu-id="5e828-106">This API has a [known issue](/graph/known-issues#incomplete-objects-when-using-getbyids-request).</span></span> <span data-ttu-id="5e828-107">Nem todos os objetos de diretório retornados são os objetos completos que contêm todas as propriedades.</span><span class="sxs-lookup"><span data-stu-id="5e828-107">Not all directory objects returned are the full objects containing all their properties.</span></span>

<span data-ttu-id="5e828-108">Alguns usos comuns dessa função são:</span><span class="sxs-lookup"><span data-stu-id="5e828-108">Some common uses for this function are to:</span></span>

* <span data-ttu-id="5e828-109">Resolva as IDs retornadas por funções (que retornam coleções de IDs) como [getMemberObjects](directoryobject-getmemberobjects.md) ou [getMemberGroups](directoryobject-getmembergroups.md) para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="5e828-109">Resolve IDs returned by functions (that return collections of IDs) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="5e828-110">Resolva IDs que persistem em um repositório externo pelo aplicativo para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="5e828-110">Resolve IDs persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e828-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e828-111">Permissions</span></span>

<span data-ttu-id="5e828-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e828-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5e828-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e828-114">Permission type</span></span>      | <span data-ttu-id="5e828-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e828-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e828-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e828-116">Delegated (work or school account)</span></span> | <span data-ttu-id="5e828-117">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5e828-117">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5e828-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e828-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e828-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e828-119">Not supported.</span></span>    |
|<span data-ttu-id="5e828-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e828-120">Application</span></span> | <span data-ttu-id="5e828-121">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e828-121">Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="5e828-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e828-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="5e828-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e828-123">Request headers</span></span>

| <span data-ttu-id="5e828-124">Nome</span><span class="sxs-lookup"><span data-stu-id="5e828-124">Name</span></span>       | <span data-ttu-id="5e828-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e828-125">Type</span></span> | <span data-ttu-id="5e828-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e828-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5e828-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e828-127">Authorization</span></span>  | <span data-ttu-id="5e828-128">string</span><span class="sxs-lookup"><span data-stu-id="5e828-128">string</span></span>  | <span data-ttu-id="5e828-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e828-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5e828-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="5e828-131">Content-type</span></span>  | <span data-ttu-id="5e828-132">string</span><span class="sxs-lookup"><span data-stu-id="5e828-132">string</span></span> | <span data-ttu-id="5e828-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e828-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5e828-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e828-135">Request body</span></span>

<span data-ttu-id="5e828-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e828-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5e828-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5e828-137">Parameter</span></span>   | <span data-ttu-id="5e828-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e828-138">Type</span></span> |<span data-ttu-id="5e828-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e828-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e828-140">ids</span><span class="sxs-lookup"><span data-stu-id="5e828-140">ids</span></span>|<span data-ttu-id="5e828-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e828-141">String collection</span></span>| <span data-ttu-id="5e828-142">Uma coleção de IDs para a qual retornar objetos.</span><span class="sxs-lookup"><span data-stu-id="5e828-142">A collection of IDs for which to return objects.</span></span>  <span data-ttu-id="5e828-143">As IDs são GUIDs, representadas como cadeias de caracteres.</span><span class="sxs-lookup"><span data-stu-id="5e828-143">The IDs are GUIDs, represented as strings.</span></span>  <span data-ttu-id="5e828-144">Você pode especificar até 1000 IDs.</span><span class="sxs-lookup"><span data-stu-id="5e828-144">You can specify up to 1000 IDs.</span></span> |
|<span data-ttu-id="5e828-145">tipos</span><span class="sxs-lookup"><span data-stu-id="5e828-145">types</span></span>|<span data-ttu-id="5e828-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e828-146">String collection</span></span>| <span data-ttu-id="5e828-147">Uma coleção de tipos de recursos que especifica o conjunto de coleções de recursos para pesquisar.</span><span class="sxs-lookup"><span data-stu-id="5e828-147">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="5e828-148">Se não estiver especificado, o padrão será [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), que contém todos os tipos de recursos definidos no diretório.</span><span class="sxs-lookup"><span data-stu-id="5e828-148">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="5e828-149">Qualquer objeto deriva do [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) pode ser especificado na coleção. Por exemplo: [usuário](/graph/api/resources/user?view=graph-rest-v1.0), [grupo](/graph/api/resources/group?view=graph-rest-v1.0), [dispositivo](/graph/api/resources/device?view=graph-rest-v1.0) e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="5e828-149">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0), and so on.</span></span> <span data-ttu-id="5e828-150">Para procurar referências para uma organização parceira do [Provedor de soluções de nuvem](https://partner.microsoft.com/cloud-solution-provider) especifique [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="5e828-150">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span></span> <span data-ttu-id="5e828-151">Se não for especificado, o padrão é [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0),  que contém todos os tipos de recursos definidos no diretório, exceto referências a uma organização parceira do [Provedor de soluções de nuvem](https://partner.microsoft.com/cloud-solution-provider).</span><span class="sxs-lookup"><span data-stu-id="5e828-151">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="5e828-152">Os valores não diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="5e828-152">The values are not case sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="5e828-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e828-153">Response</span></span>

<span data-ttu-id="5e828-154">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e828-154">If successful, this method returns a `200 OK` response code and a string collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e828-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e828-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e828-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e828-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5e828-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e828-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/v1.0/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893874940a3-97b7-68513b600544","5d6059b6368d-45f8-91e18e07d485f1d0"],
    "types":["user"]
}
```
# <a name="c"></a>[<span data-ttu-id="5e828-158">C#</span><span class="sxs-lookup"><span data-stu-id="5e828-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e828-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e828-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e828-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e828-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5e828-161">Java</span><span class="sxs-lookup"><span data-stu-id="5e828-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5e828-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e828-162">Response</span></span>

><span data-ttu-id="5e828-163">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5e828-163">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
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
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

