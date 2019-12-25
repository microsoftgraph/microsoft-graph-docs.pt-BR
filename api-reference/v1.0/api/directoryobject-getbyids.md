---
title: Obter objetos directory a partir de uma lista de ids
description: A opção selecionar não está disponível para todos os tipos de arquivo.
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 57037df3121a101caa4ee8e55ecf763b2a562e1a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869939"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="52580-103">Obter objetos directory a partir de uma lista de ids</span><span class="sxs-lookup"><span data-stu-id="52580-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="52580-104">Retorna os objetos de diretório especificados em uma lista de IDs.</span><span class="sxs-lookup"><span data-stu-id="52580-104">Returns the directory objects specified in a list of IDs.</span></span>

>[!NOTE]
><span data-ttu-id="52580-105">Os objetos de diretório retornados são os objetos completos que contêm todas as propriedades.</span><span class="sxs-lookup"><span data-stu-id="52580-105">The directory objects returned are the full objects containing all their properties.</span></span> <span data-ttu-id="52580-106">A opção `$select` não está disponível para esta operação.</span><span class="sxs-lookup"><span data-stu-id="52580-106">The `$select` query option is not available for this operation.</span></span>

>[!NOTE]
><span data-ttu-id="52580-107">Essa API tem um [problema conhecido](/graph/known-issues#incomplete-objects-when-using-getbyids-request).</span><span class="sxs-lookup"><span data-stu-id="52580-107">This API has a [known issue](/graph/known-issues#incomplete-objects-when-using-getbyids-request).</span></span> <span data-ttu-id="52580-108">Nem todos os objetos de diretório retornados são os objetos completos que contêm todas as propriedades.</span><span class="sxs-lookup"><span data-stu-id="52580-108">Not all directory objects returned are the full objects containing all their properties.</span></span>

<span data-ttu-id="52580-109">Alguns usos comuns dessa função são:</span><span class="sxs-lookup"><span data-stu-id="52580-109">Some common uses for this function are to:</span></span>

* <span data-ttu-id="52580-110">Resolva as IDs retornadas por funções (que retornam coleções de IDs) como [getMemberObjects](directoryobject-getmemberobjects.md) ou [getMemberGroups](directoryobject-getmembergroups.md) para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="52580-110">Resolve IDs returned by functions (that return collections of IDs) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="52580-111">Resolver ids que persistem em um repositório externo pelo aplicativo para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="52580-111">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="52580-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="52580-112">Permissions</span></span>

<span data-ttu-id="52580-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52580-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="52580-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52580-115">Permission type</span></span>      | <span data-ttu-id="52580-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52580-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52580-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52580-117">Delegated (work or school account)</span></span> | <span data-ttu-id="52580-118">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="52580-118">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="52580-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52580-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52580-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52580-120">Not supported.</span></span>    |
|<span data-ttu-id="52580-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52580-121">Application</span></span> | <span data-ttu-id="52580-122">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="52580-122">Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="52580-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52580-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="52580-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52580-124">Request headers</span></span>

| <span data-ttu-id="52580-125">Nome</span><span class="sxs-lookup"><span data-stu-id="52580-125">Name</span></span>       | <span data-ttu-id="52580-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="52580-126">Type</span></span> | <span data-ttu-id="52580-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="52580-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="52580-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="52580-128">Authorization</span></span>  | <span data-ttu-id="52580-129">string</span><span class="sxs-lookup"><span data-stu-id="52580-129">string</span></span>  | <span data-ttu-id="52580-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52580-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52580-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="52580-132">Content-Type</span></span>  | <span data-ttu-id="52580-133">string</span><span class="sxs-lookup"><span data-stu-id="52580-133">string</span></span> | <span data-ttu-id="52580-134">application/json</span><span class="sxs-lookup"><span data-stu-id="52580-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="52580-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52580-135">Request body</span></span>

<span data-ttu-id="52580-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52580-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="52580-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="52580-137">Parameter</span></span>   | <span data-ttu-id="52580-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="52580-138">Type</span></span> |<span data-ttu-id="52580-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="52580-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52580-140">ids</span><span class="sxs-lookup"><span data-stu-id="52580-140">ids</span></span>|<span data-ttu-id="52580-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="52580-141">String collection</span></span>| <span data-ttu-id="52580-142">Uma coleção de IDs para a qual retornar objetos.</span><span class="sxs-lookup"><span data-stu-id="52580-142">A collection of IDs for which to return objects.</span></span> <span data-ttu-id="52580-143">Você pode especificar até 1000 IDs.</span><span class="sxs-lookup"><span data-stu-id="52580-143">You can specify up to 1000 IDs.</span></span> |
|<span data-ttu-id="52580-144">tipos</span><span class="sxs-lookup"><span data-stu-id="52580-144">types</span></span>|<span data-ttu-id="52580-145">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="52580-145">String collection</span></span>| <span data-ttu-id="52580-146">Uma coleção de tipos de recursos que especifica o conjunto de coleções de recursos para pesquisar.</span><span class="sxs-lookup"><span data-stu-id="52580-146">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="52580-147">Se não estiver especificado, o padrão será [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), que contém todos os tipos de recursos definidos no diretório.</span><span class="sxs-lookup"><span data-stu-id="52580-147">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="52580-148">Qualquer objeto deriva do [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) pode ser especificado na coleção. Por exemplo: [usuário](/graph/api/resources/user?view=graph-rest-v1.0), [grupo](/graph/api/resources/group?view=graph-rest-v1.0), [dispositivo](/graph/api/resources/device?view=graph-rest-v1.0) e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="52580-148">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0), and so on.</span></span> <span data-ttu-id="52580-149">Para procurar referências para uma organização parceira do [Provedor de soluções de nuvem](https://partner.microsoft.com/pt-BR/cloud-solution-provider) especifique [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="52580-149">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/pt-BR/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span></span> <span data-ttu-id="52580-150">Se não for especificado, o padrão é [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0),  que contém todos os tipos de recursos definidos no diretório, exceto referências a uma organização parceira do [Provedor de soluções de nuvem](https://partner.microsoft.com/pt-BR/cloud-solution-provider).</span><span class="sxs-lookup"><span data-stu-id="52580-150">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/pt-BR/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="52580-151">Os valores não diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="52580-151">The values are not case sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="52580-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="52580-152">Response</span></span>

<span data-ttu-id="52580-153">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52580-153">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52580-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52580-154">Example</span></span>

##### <a name="request"></a><span data-ttu-id="52580-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52580-155">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="52580-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="52580-156">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="52580-157">C#</span><span class="sxs-lookup"><span data-stu-id="52580-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52580-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52580-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="52580-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52580-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="52580-160">Java</span><span class="sxs-lookup"><span data-stu-id="52580-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="52580-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="52580-161">Response</span></span>

<span data-ttu-id="52580-p107">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52580-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
