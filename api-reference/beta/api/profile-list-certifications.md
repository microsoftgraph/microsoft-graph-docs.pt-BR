---
title: Listar certificações
description: Obtenha uma coleção de personCertifications da propriedade de navegação certificações.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: fd7f8196bf0b76ce16d1949d7e46c1d751a7f0db
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819334"
---
# <a name="list-certifications"></a><span data-ttu-id="b6eb2-103">Listar certificações</span><span class="sxs-lookup"><span data-stu-id="b6eb2-103">List certifications</span></span>
<span data-ttu-id="b6eb2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6eb2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b6eb2-105">Recupere uma lista de objetos [personCertification](../resources/personcertification.md) de um [perfil](../resources/profile.md)de usuário.</span><span class="sxs-lookup"><span data-stu-id="b6eb2-105">Retrieve a list of [personCertification](../resources/personcertification.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b6eb2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6eb2-106">Permissions</span></span>

<span data-ttu-id="b6eb2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6eb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b6eb2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6eb2-109">Permission type</span></span>                        | <span data-ttu-id="b6eb2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6eb2-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="b6eb2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6eb2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b6eb2-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b6eb2-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b6eb2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6eb2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6eb2-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b6eb2-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b6eb2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6eb2-115">Application</span></span>                            | <span data-ttu-id="b6eb2-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b6eb2-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="b6eb2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6eb2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/certifications
GET /users/{id | userPrincipalName}/profile/certifications
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6eb2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b6eb2-118">Optional query parameters</span></span>

<span data-ttu-id="b6eb2-119">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b6eb2-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="b6eb2-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b6eb2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="b6eb2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b6eb2-121">Name</span></span>            |<span data-ttu-id="b6eb2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b6eb2-122">Value</span></span>    |<span data-ttu-id="b6eb2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6eb2-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="b6eb2-124">$filter</span><span class="sxs-lookup"><span data-stu-id="b6eb2-124">$filter</span></span>         |<span data-ttu-id="b6eb2-125">string</span><span class="sxs-lookup"><span data-stu-id="b6eb2-125">string</span></span>   |<span data-ttu-id="b6eb2-126">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="b6eb2-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="b6eb2-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="b6eb2-127">$orderby</span></span>        |<span data-ttu-id="b6eb2-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6eb2-128">string</span></span>   |<span data-ttu-id="b6eb2-129">Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="b6eb2-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="b6eb2-130">Você pode alterar a ordem da resposta usando o parâmetro *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="b6eb2-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="b6eb2-131">$select</span><span class="sxs-lookup"><span data-stu-id="b6eb2-131">$select</span></span>         |<span data-ttu-id="b6eb2-132">string</span><span class="sxs-lookup"><span data-stu-id="b6eb2-132">string</span></span>   |<span data-ttu-id="b6eb2-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="b6eb2-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="b6eb2-135">$skip</span><span class="sxs-lookup"><span data-stu-id="b6eb2-135">$skip</span></span>           |<span data-ttu-id="b6eb2-136">int</span><span class="sxs-lookup"><span data-stu-id="b6eb2-136">int</span></span>      |<span data-ttu-id="b6eb2-137">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="b6eb2-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="b6eb2-138">$top</span><span class="sxs-lookup"><span data-stu-id="b6eb2-138">$top</span></span>            |<span data-ttu-id="b6eb2-139">int</span><span class="sxs-lookup"><span data-stu-id="b6eb2-139">int</span></span>      |<span data-ttu-id="b6eb2-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="b6eb2-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="b6eb2-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6eb2-141">Request headers</span></span>
|<span data-ttu-id="b6eb2-142">Nome</span><span class="sxs-lookup"><span data-stu-id="b6eb2-142">Name</span></span>|<span data-ttu-id="b6eb2-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6eb2-143">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b6eb2-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6eb2-144">Authorization</span></span>|<span data-ttu-id="b6eb2-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6eb2-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6eb2-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6eb2-147">Request body</span></span>
<span data-ttu-id="b6eb2-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6eb2-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6eb2-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6eb2-149">Response</span></span>

<span data-ttu-id="b6eb2-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [personCertification](../resources/personcertification.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6eb2-150">If successful, this method returns a `200 OK` response code and a collection of [personCertification](../resources/personcertification.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b6eb2-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b6eb2-151">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="b6eb2-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6eb2-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itemcertifications_from_profile"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/certifications
```
# <a name="c"></a>[<span data-ttu-id="b6eb2-153">C#</span><span class="sxs-lookup"><span data-stu-id="b6eb2-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-itemcertifications-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6eb2-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6eb2-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-itemcertifications-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6eb2-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6eb2-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-itemcertifications-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b6eb2-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6eb2-156">Response</span></span>
<span data-ttu-id="b6eb2-157">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b6eb2-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.personCertification)"
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
      "source": null,
      "certificationId": "KB-1235466333663322",
      "description": "Blackbelt in Marketing - Brand Management",
      "displayName": "Marketing Blackbelt - Brand Management",
      "endDate": "Date",
      "issuedDate": "Date",
      "issuingAuthority": "International Academy of Marketing Excellence",
      "issuingCompany": "International Academy of Marketing Excellence",
      "startDate": "Date",
      "thumbnailUrl": "https://iame.io/dfhdfdfd334.jpg",
      "webUrl": "https://www.iame.io/blackbelt"
    }
  ]
}
```