---
title: Obter objetos directory a partir de uma lista de ids
description: A opção selecionar não está disponível para todos os tipos de arquivo.
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9804a2395205e34f6371534b167a9de1efb29a2b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272377"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="0bcfa-103">Obter objetos directory a partir de uma lista de ids</span><span class="sxs-lookup"><span data-stu-id="0bcfa-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="0bcfa-p101">Retorna os objetos directory especificados a partir de uma lista de ids  OBSERVAÇÃO: Os objetos de diretório retornados são os objetos completos que contêm **todas** as propriedades. A opção `$select` não está disponível para todos os tipos de arquivo.</span><span class="sxs-lookup"><span data-stu-id="0bcfa-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="0bcfa-107">Alguns usos comuns dessa função são:</span><span class="sxs-lookup"><span data-stu-id="0bcfa-107">Some common uses for this function are to:</span></span>

* <span data-ttu-id="0bcfa-108">Resolver ids retornadas por funções (que retornam coleções de ids) como [getMemberObjects](directoryobject-getmemberobjects.md) ou [getMemberGroups](directoryobject-getmembergroups.md) para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="0bcfa-108">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="0bcfa-109">Resolver ids que persistem em um repositório externo pelo aplicativo para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="0bcfa-109">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0bcfa-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="0bcfa-110">Permissions</span></span>

<span data-ttu-id="0bcfa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bcfa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0bcfa-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0bcfa-113">Permission type</span></span>      | <span data-ttu-id="0bcfa-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0bcfa-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bcfa-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0bcfa-115">Delegated (work or school account)</span></span> | <span data-ttu-id="0bcfa-116">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0bcfa-116">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0bcfa-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0bcfa-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bcfa-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bcfa-118">Not supported.</span></span>    |
|<span data-ttu-id="0bcfa-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0bcfa-119">Application</span></span> | <span data-ttu-id="0bcfa-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bcfa-120">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bcfa-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0bcfa-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="0bcfa-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0bcfa-122">Request headers</span></span>

| <span data-ttu-id="0bcfa-123">Nome</span><span class="sxs-lookup"><span data-stu-id="0bcfa-123">Name</span></span>       | <span data-ttu-id="0bcfa-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bcfa-124">Type</span></span> | <span data-ttu-id="0bcfa-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bcfa-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0bcfa-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="0bcfa-126">Authorization</span></span>  | <span data-ttu-id="0bcfa-127">string</span><span class="sxs-lookup"><span data-stu-id="0bcfa-127">string</span></span>  | <span data-ttu-id="0bcfa-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0bcfa-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0bcfa-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0bcfa-130">Content-Type</span></span>  | <span data-ttu-id="0bcfa-131">string</span><span class="sxs-lookup"><span data-stu-id="0bcfa-131">string</span></span> | <span data-ttu-id="0bcfa-132">application/json</span><span class="sxs-lookup"><span data-stu-id="0bcfa-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0bcfa-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0bcfa-133">Request body</span></span>

<span data-ttu-id="0bcfa-134">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0bcfa-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0bcfa-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0bcfa-135">Parameter</span></span>   | <span data-ttu-id="0bcfa-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bcfa-136">Type</span></span> |<span data-ttu-id="0bcfa-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bcfa-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0bcfa-138">ids</span><span class="sxs-lookup"><span data-stu-id="0bcfa-138">ids</span></span>|<span data-ttu-id="0bcfa-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bcfa-139">String collection</span></span>| <span data-ttu-id="0bcfa-p104">Uma coleção de ids para a qual retornar objetos. Você pode especificar até 1000 ids.</span><span class="sxs-lookup"><span data-stu-id="0bcfa-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="0bcfa-142">tipos</span><span class="sxs-lookup"><span data-stu-id="0bcfa-142">types</span></span>|<span data-ttu-id="0bcfa-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bcfa-143">String collection</span></span>| <span data-ttu-id="0bcfa-144">Uma coleção de tipos de recursos que especifica o conjunto de coleções de recursos para pesquisar.</span><span class="sxs-lookup"><span data-stu-id="0bcfa-144">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="0bcfa-145">Se não estiver especificado, o padrão será [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), que contém todos os tipos de recursos definidos no diretório.</span><span class="sxs-lookup"><span data-stu-id="0bcfa-145">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="0bcfa-146">Qualquer objeto deriva do [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) pode ser especificado na coleção. Por exemplo: [usuário](/graph/api/resources/user?view=graph-rest-v1.0), [grupo](/graph/api/resources/group?view=graph-rest-v1.0), [dispositivo](/graph/api/resources/device?view=graph-rest-v1.0) e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="0bcfa-146">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0), and so on.</span></span> <span data-ttu-id="0bcfa-147">Para procurar referências para uma organização parceira do [Provedor de soluções de nuvem](https://partner.microsoft.com/en-us/cloud-solution-provider) especifique [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="0bcfa-147">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span></span> <span data-ttu-id="0bcfa-148">Se não for especificado, o padrão é [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0),  que contém todos os tipos de recursos definidos no diretório, exceto referências a uma organização parceira do [Provedor de soluções de nuvem](https://partner.microsoft.com/en-us/cloud-solution-provider).</span><span class="sxs-lookup"><span data-stu-id="0bcfa-148">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="0bcfa-149">Os valores não diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="0bcfa-149">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="0bcfa-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bcfa-150">Response</span></span>

<span data-ttu-id="0bcfa-151">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0bcfa-151">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bcfa-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0bcfa-152">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0bcfa-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0bcfa-153">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="0bcfa-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bcfa-154">Response</span></span>

<span data-ttu-id="0bcfa-p106">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0bcfa-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0bcfa-157">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="0bcfa-157">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0bcfa-158">C#</span><span class="sxs-lookup"><span data-stu-id="0bcfa-158">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/directoryobject_getById-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0bcfa-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="0bcfa-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/directoryobject_getById-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0bcfa-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0bcfa-160">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/directoryobject_getById-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryobject-getbyids.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directoryobject-getbyids.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryobject-getbyids.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
