---
title: Obter objetos directory a partir de uma lista de ids
description: A opção selecionar não está disponível para todos os tipos de arquivo.
author: keylimesoda
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8ff81002804a445ab102b3df0bac2b57332fec2b
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181927"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="2cea6-103">Obter objetos directory a partir de uma lista de ids</span><span class="sxs-lookup"><span data-stu-id="2cea6-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="2cea6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cea6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2cea6-105">Retorna os objetos de diretório especificados em uma lista de IDs.</span><span class="sxs-lookup"><span data-stu-id="2cea6-105">Returns the directory objects specified in a list of IDs.</span></span>

>[!NOTE]
><span data-ttu-id="2cea6-106">Os objetos de diretório retornados são os objetos completos que contêm todas as propriedades.</span><span class="sxs-lookup"><span data-stu-id="2cea6-106">The directory objects returned are the full objects containing all their properties.</span></span> <span data-ttu-id="2cea6-107">A opção `$select` não está disponível para esta operação.</span><span class="sxs-lookup"><span data-stu-id="2cea6-107">The `$select` query option is not available for this operation.</span></span>

>[!NOTE]
><span data-ttu-id="2cea6-108">Essa API tem um [problema conhecido](/graph/known-issues#incomplete-objects-when-using-getbyids-request).</span><span class="sxs-lookup"><span data-stu-id="2cea6-108">This API has a [known issue](/graph/known-issues#incomplete-objects-when-using-getbyids-request).</span></span> <span data-ttu-id="2cea6-109">Nem todos os objetos de diretório retornados são os objetos completos que contêm todas as propriedades.</span><span class="sxs-lookup"><span data-stu-id="2cea6-109">Not all directory objects returned are the full objects containing all their properties.</span></span>

<span data-ttu-id="2cea6-110">Alguns usos comuns dessa função são:</span><span class="sxs-lookup"><span data-stu-id="2cea6-110">Some common uses for this function are to:</span></span>

* <span data-ttu-id="2cea6-111">Resolva as IDs retornadas por funções (que retornam coleções de IDs) como [getMemberObjects](directoryobject-getmemberobjects.md) ou [getMemberGroups](directoryobject-getmembergroups.md) para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="2cea6-111">Resolve IDs returned by functions (that return collections of IDs) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="2cea6-112">Resolver ids que persistem em um repositório externo pelo aplicativo para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="2cea6-112">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="2cea6-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="2cea6-113">Permissions</span></span>

<span data-ttu-id="2cea6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cea6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2cea6-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2cea6-116">Permission type</span></span>      | <span data-ttu-id="2cea6-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2cea6-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2cea6-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2cea6-118">Delegated (work or school account)</span></span> | <span data-ttu-id="2cea6-119">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2cea6-119">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2cea6-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2cea6-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2cea6-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2cea6-121">Not supported.</span></span>    |
|<span data-ttu-id="2cea6-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2cea6-122">Application</span></span> | <span data-ttu-id="2cea6-123">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2cea6-123">Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="2cea6-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2cea6-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="2cea6-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2cea6-125">Request headers</span></span>

| <span data-ttu-id="2cea6-126">Nome</span><span class="sxs-lookup"><span data-stu-id="2cea6-126">Name</span></span>       | <span data-ttu-id="2cea6-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cea6-127">Type</span></span> | <span data-ttu-id="2cea6-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cea6-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2cea6-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="2cea6-129">Authorization</span></span>  | <span data-ttu-id="2cea6-130">string</span><span class="sxs-lookup"><span data-stu-id="2cea6-130">string</span></span>  | <span data-ttu-id="2cea6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2cea6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2cea6-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2cea6-133">Content-Type</span></span>  | <span data-ttu-id="2cea6-134">string</span><span class="sxs-lookup"><span data-stu-id="2cea6-134">string</span></span> | <span data-ttu-id="2cea6-135">application/json</span><span class="sxs-lookup"><span data-stu-id="2cea6-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2cea6-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2cea6-136">Request body</span></span>

<span data-ttu-id="2cea6-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2cea6-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2cea6-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2cea6-138">Parameter</span></span>   | <span data-ttu-id="2cea6-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cea6-139">Type</span></span> |<span data-ttu-id="2cea6-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cea6-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2cea6-141">ids</span><span class="sxs-lookup"><span data-stu-id="2cea6-141">ids</span></span>|<span data-ttu-id="2cea6-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2cea6-142">String collection</span></span>| <span data-ttu-id="2cea6-143">Uma coleção de IDs para a qual retornar objetos.</span><span class="sxs-lookup"><span data-stu-id="2cea6-143">A collection of IDs for which to return objects.</span></span> <span data-ttu-id="2cea6-144">Você pode especificar até 1000 IDs.</span><span class="sxs-lookup"><span data-stu-id="2cea6-144">You can specify up to 1000 IDs.</span></span> |
|<span data-ttu-id="2cea6-145">tipos</span><span class="sxs-lookup"><span data-stu-id="2cea6-145">types</span></span>|<span data-ttu-id="2cea6-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2cea6-146">String collection</span></span>| <span data-ttu-id="2cea6-147">Uma coleção de tipos de recursos que especifica o conjunto de coleções de recursos para pesquisar.</span><span class="sxs-lookup"><span data-stu-id="2cea6-147">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="2cea6-148">Se não estiver especificado, o padrão será [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), que contém todos os tipos de recursos definidos no diretório.</span><span class="sxs-lookup"><span data-stu-id="2cea6-148">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="2cea6-149">Qualquer objeto deriva do [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) pode ser especificado na coleção. Por exemplo: [usuário](/graph/api/resources/user?view=graph-rest-v1.0), [grupo](/graph/api/resources/group?view=graph-rest-v1.0), [dispositivo](/graph/api/resources/device?view=graph-rest-v1.0) e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="2cea6-149">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0), and so on.</span></span> <span data-ttu-id="2cea6-150">Para procurar referências para uma organização parceira do [Provedor de soluções de nuvem](https://partner.microsoft.com/pt-BR/cloud-solution-provider) especifique [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="2cea6-150">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/pt-BR/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span></span> <span data-ttu-id="2cea6-151">Se não for especificado, o padrão é [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0),  que contém todos os tipos de recursos definidos no diretório, exceto referências a uma organização parceira do [Provedor de soluções de nuvem](https://partner.microsoft.com/pt-BR/cloud-solution-provider).</span><span class="sxs-lookup"><span data-stu-id="2cea6-151">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/pt-BR/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="2cea6-152">Os valores não diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="2cea6-152">The values are not case sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="2cea6-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cea6-153">Response</span></span>

<span data-ttu-id="2cea6-154">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2cea6-154">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cea6-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2cea6-155">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2cea6-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2cea6-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2cea6-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="2cea6-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2cea6-158">C#</span><span class="sxs-lookup"><span data-stu-id="2cea6-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2cea6-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2cea6-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2cea6-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2cea6-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2cea6-161">Java</span><span class="sxs-lookup"><span data-stu-id="2cea6-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2cea6-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cea6-162">Response</span></span>

<span data-ttu-id="2cea6-p107">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2cea6-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
