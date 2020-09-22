---
title: Listar qualificações
description: Recupere uma lista de objetos skillProficiency.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: d5de0db3f1a1ba8244908100fe9f4e16765c441c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034628"
---
# <a name="list-skills"></a><span data-ttu-id="6ab25-103">Listar qualificações</span><span class="sxs-lookup"><span data-stu-id="6ab25-103">List skills</span></span>

<span data-ttu-id="6ab25-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ab25-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ab25-105">Recupere uma lista de objetos [skillProficiency](../resources/skillproficiency.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="6ab25-105">Retrieve a list of [skillProficiency](../resources/skillproficiency.md) objects in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6ab25-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6ab25-106">Permissions</span></span>

<span data-ttu-id="6ab25-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ab25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6ab25-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ab25-109">Permission type</span></span>                        | <span data-ttu-id="6ab25-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ab25-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="6ab25-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ab25-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6ab25-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6ab25-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="6ab25-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ab25-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ab25-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6ab25-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="6ab25-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ab25-115">Application</span></span>                            | <span data-ttu-id="6ab25-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6ab25-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="6ab25-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ab25-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/skills
GET /users/{id | userPrincipalName}/profile/skills
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6ab25-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6ab25-118">Optional query parameters</span></span>

<span data-ttu-id="6ab25-119">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6ab25-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="6ab25-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6ab25-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="6ab25-121">Nome</span><span class="sxs-lookup"><span data-stu-id="6ab25-121">Name</span></span>            |<span data-ttu-id="6ab25-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6ab25-122">Value</span></span>    |<span data-ttu-id="6ab25-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ab25-123">Description</span></span>                                                                                                                                                                      |
|:---------------|:--------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="6ab25-124">$filter</span><span class="sxs-lookup"><span data-stu-id="6ab25-124">$filter</span></span>         |<span data-ttu-id="6ab25-125">string</span><span class="sxs-lookup"><span data-stu-id="6ab25-125">string</span></span>   |<span data-ttu-id="6ab25-126">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="6ab25-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                                  |
|<span data-ttu-id="6ab25-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="6ab25-127">$orderby</span></span>        |<span data-ttu-id="6ab25-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ab25-128">string</span></span>   |<span data-ttu-id="6ab25-129">Por padrão, os objetos na resposta são classificados por seu valor **createdDateTime** em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="6ab25-129">By default, the objects in the response are sorted by their **createdDateTime** value in a query.</span></span> <span data-ttu-id="6ab25-130">Você pode alterar a ordem da resposta usando o `$orderby` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="6ab25-130">You can change the order of the of the response using the `$orderby` parameter.</span></span>|
|<span data-ttu-id="6ab25-131">$select</span><span class="sxs-lookup"><span data-stu-id="6ab25-131">$select</span></span>         |<span data-ttu-id="6ab25-132">string</span><span class="sxs-lookup"><span data-stu-id="6ab25-132">string</span></span>   |<span data-ttu-id="6ab25-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="6ab25-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                             |
|<span data-ttu-id="6ab25-135">$skip</span><span class="sxs-lookup"><span data-stu-id="6ab25-135">$skip</span></span>           |<span data-ttu-id="6ab25-136">int</span><span class="sxs-lookup"><span data-stu-id="6ab25-136">int</span></span>      |<span data-ttu-id="6ab25-137">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="6ab25-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                     |
|<span data-ttu-id="6ab25-138">$top</span><span class="sxs-lookup"><span data-stu-id="6ab25-138">$top</span></span>            |<span data-ttu-id="6ab25-139">int</span><span class="sxs-lookup"><span data-stu-id="6ab25-139">int</span></span>      |<span data-ttu-id="6ab25-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="6ab25-140">Number of results to be returned.</span></span>                                                                                                                                                |

## <a name="request-headers"></a><span data-ttu-id="6ab25-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ab25-141">Request headers</span></span>

| <span data-ttu-id="6ab25-142">Nome</span><span class="sxs-lookup"><span data-stu-id="6ab25-142">Name</span></span>           |<span data-ttu-id="6ab25-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ab25-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="6ab25-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ab25-144">Authorization</span></span>  | <span data-ttu-id="6ab25-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ab25-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="6ab25-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6ab25-147">Content-Type</span></span>   | <span data-ttu-id="6ab25-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ab25-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ab25-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ab25-150">Request body</span></span>

<span data-ttu-id="6ab25-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6ab25-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ab25-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ab25-152">Response</span></span>

<span data-ttu-id="6ab25-153">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [skillProficiency](../resources/skillproficiency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ab25-153">If successful, this method returns a `200 OK` response code and a collection of [skillProficiency](../resources/skillproficiency.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6ab25-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6ab25-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6ab25-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ab25-155">Request</span></span>

<span data-ttu-id="6ab25-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ab25-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6ab25-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ab25-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_skills"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/skills
```
# <a name="c"></a>[<span data-ttu-id="6ab25-158">C#</span><span class="sxs-lookup"><span data-stu-id="6ab25-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-skills-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ab25-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ab25-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-skills-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ab25-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ab25-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-skills-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6ab25-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ab25-161">Response</span></span>

<span data-ttu-id="6ab25-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6ab25-162">The following is an example of the response.</span></span>

> <span data-ttu-id="6ab25-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ab25-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skillProficiency",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
      "source": null,
      "categories": [
        "Professional"
      ],
      "displayName": "API Design",
      "proficiency": "advancedProfessional",
      "webUrl": null,
      "collaborationTags": [
        "ableToMentor"
      ]
    }
  ]
}
```


