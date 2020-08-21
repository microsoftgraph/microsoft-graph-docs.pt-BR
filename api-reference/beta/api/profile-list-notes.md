---
title: Listar anotações
description: Obtenha o personAnnotations da propriedade de navegação Notes.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a6cb5eecdd6d779ed89cde263135def3f682c12f
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819369"
---
# <a name="list-notes"></a><span data-ttu-id="b8659-103">Listar anotações</span><span class="sxs-lookup"><span data-stu-id="b8659-103">List notes</span></span>
<span data-ttu-id="b8659-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8659-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b8659-105">Recupere uma lista de objetos [personAnnotation](../resources/personinterest.md) de um [perfil](../resources/profile.md)de usuário.</span><span class="sxs-lookup"><span data-stu-id="b8659-105">Retrieve a list of [personAnnotation](../resources/personinterest.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b8659-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8659-106">Permissions</span></span>

<span data-ttu-id="b8659-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8659-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8659-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8659-109">Permission type</span></span>                        | <span data-ttu-id="b8659-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8659-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="b8659-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8659-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8659-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b8659-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b8659-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8659-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8659-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b8659-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b8659-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8659-115">Application</span></span>                            | <span data-ttu-id="b8659-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b8659-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="b8659-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8659-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/notes
GET /users/{id | userPrincipalName}/profile/notes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8659-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b8659-118">Optional query parameters</span></span>

<span data-ttu-id="b8659-119">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b8659-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="b8659-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b8659-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="b8659-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b8659-121">Name</span></span>            |<span data-ttu-id="b8659-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b8659-122">Value</span></span>    |<span data-ttu-id="b8659-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8659-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="b8659-124">$filter</span><span class="sxs-lookup"><span data-stu-id="b8659-124">$filter</span></span>         |<span data-ttu-id="b8659-125">string</span><span class="sxs-lookup"><span data-stu-id="b8659-125">string</span></span>   |<span data-ttu-id="b8659-126">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="b8659-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="b8659-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="b8659-127">$orderby</span></span>        |<span data-ttu-id="b8659-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8659-128">string</span></span>   |<span data-ttu-id="b8659-129">Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="b8659-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="b8659-130">Você pode alterar a ordem da resposta usando o parâmetro *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="b8659-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="b8659-131">$select</span><span class="sxs-lookup"><span data-stu-id="b8659-131">$select</span></span>         |<span data-ttu-id="b8659-132">string</span><span class="sxs-lookup"><span data-stu-id="b8659-132">string</span></span>   |<span data-ttu-id="b8659-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="b8659-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="b8659-135">$skip</span><span class="sxs-lookup"><span data-stu-id="b8659-135">$skip</span></span>           |<span data-ttu-id="b8659-136">int</span><span class="sxs-lookup"><span data-stu-id="b8659-136">int</span></span>      |<span data-ttu-id="b8659-137">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="b8659-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="b8659-138">$top</span><span class="sxs-lookup"><span data-stu-id="b8659-138">$top</span></span>            |<span data-ttu-id="b8659-139">int</span><span class="sxs-lookup"><span data-stu-id="b8659-139">int</span></span>      |<span data-ttu-id="b8659-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="b8659-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="b8659-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8659-141">Request headers</span></span>
|<span data-ttu-id="b8659-142">Nome</span><span class="sxs-lookup"><span data-stu-id="b8659-142">Name</span></span>|<span data-ttu-id="b8659-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8659-143">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b8659-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8659-144">Authorization</span></span>|<span data-ttu-id="b8659-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8659-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8659-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8659-147">Request body</span></span>
<span data-ttu-id="b8659-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8659-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8659-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8659-149">Response</span></span>

<span data-ttu-id="b8659-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [personAnnotation](../resources/personannotation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8659-150">If successful, this method returns a `200 OK` response code and a collection of [personAnnotation](../resources/personannotation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b8659-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b8659-151">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="b8659-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8659-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_notes"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/notes
```
# <a name="c"></a>[<span data-ttu-id="b8659-153">C#</span><span class="sxs-lookup"><span data-stu-id="b8659-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-notes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b8659-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8659-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-notes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b8659-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8659-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-notes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b8659-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8659-156">Response</span></span>
<span data-ttu-id="b8659-157">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b8659-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.personAnnotation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
      "allowedAudiences": "organization",
      "inference": null,
      "createdDateTime": "2020-07-06T06:34:12.2294868Z",
      "createdBy": {
        "application": null,
        "device": null,
        "user": {
          "displayName": "Innocenty Popov",
          "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
        }
      },
      "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
      "lastModifiedBy": {
        "application": null,
        "device": null,
        "user": {
          "displayName": "Innocenty Popov",
          "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
        }
      },
      "detail": {
        "contentType": "text",
        "content": "I am originally from Australia, but grew up in Moscow."
      },
      "displayName": "About Me"
    }
  ]
}
```
