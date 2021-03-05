---
title: Listar contas
description: Recupere uma lista de objetos userAccountInformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ded9150c3896f1b10c0ba0ac9077c4d3aae209ad
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474838"
---
# <a name="list-accounts"></a><span data-ttu-id="d1578-103">Listar contas</span><span class="sxs-lookup"><span data-stu-id="d1578-103">List accounts</span></span>

<span data-ttu-id="d1578-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1578-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1578-105">Recupera propriedades relacionadas às contas do usuário do [perfil](../resources/profile.md).</span><span class="sxs-lookup"><span data-stu-id="d1578-105">Retrieves properties related to the user's accounts from the [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d1578-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1578-106">Permissions</span></span>

<span data-ttu-id="d1578-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1578-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d1578-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1578-109">Permission type</span></span>                        | <span data-ttu-id="d1578-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1578-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="d1578-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1578-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1578-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1578-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d1578-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1578-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1578-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1578-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d1578-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1578-115">Application</span></span>                            | <span data-ttu-id="d1578-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1578-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="d1578-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1578-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/account
GET /users/{id | userPrincipalName}/profile/account
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1578-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d1578-118">Optional query parameters</span></span>

<span data-ttu-id="d1578-119">Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d1578-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="d1578-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d1578-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="d1578-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d1578-121">Name</span></span>            |<span data-ttu-id="d1578-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d1578-122">Value</span></span>    |<span data-ttu-id="d1578-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1578-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="d1578-124">$filter</span><span class="sxs-lookup"><span data-stu-id="d1578-124">$filter</span></span>         |<span data-ttu-id="d1578-125">string</span><span class="sxs-lookup"><span data-stu-id="d1578-125">string</span></span>   |<span data-ttu-id="d1578-126">Limita a resposta apenas aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="d1578-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="d1578-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="d1578-127">$orderby</span></span>        |<span data-ttu-id="d1578-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1578-128">string</span></span>   |<span data-ttu-id="d1578-129">Por padrão, os objetos na resposta são classificação pelo valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="d1578-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="d1578-130">Você pode alterar a ordem da resposta usando o parâmetro *$orderby.*</span><span class="sxs-lookup"><span data-stu-id="d1578-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="d1578-131">$select</span><span class="sxs-lookup"><span data-stu-id="d1578-131">$select</span></span>         |<span data-ttu-id="d1578-132">string</span><span class="sxs-lookup"><span data-stu-id="d1578-132">string</span></span>   |<span data-ttu-id="d1578-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="d1578-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="d1578-135">$skip</span><span class="sxs-lookup"><span data-stu-id="d1578-135">$skip</span></span>           |<span data-ttu-id="d1578-136">int</span><span class="sxs-lookup"><span data-stu-id="d1578-136">int</span></span>      |<span data-ttu-id="d1578-137">Ignore os primeiros resultados n, úteis para pajamento.</span><span class="sxs-lookup"><span data-stu-id="d1578-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="d1578-138">$top</span><span class="sxs-lookup"><span data-stu-id="d1578-138">$top</span></span>            |<span data-ttu-id="d1578-139">int</span><span class="sxs-lookup"><span data-stu-id="d1578-139">int</span></span>      |<span data-ttu-id="d1578-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="d1578-140">Number of results to be returned.</span></span>                                                                                                                                           |


## <a name="request-headers"></a><span data-ttu-id="d1578-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1578-141">Request headers</span></span>

| <span data-ttu-id="d1578-142">Nome</span><span class="sxs-lookup"><span data-stu-id="d1578-142">Name</span></span>           |<span data-ttu-id="d1578-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1578-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="d1578-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1578-144">Authorization</span></span>  | <span data-ttu-id="d1578-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1578-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="d1578-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d1578-147">Content-Type</span></span>   | <span data-ttu-id="d1578-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1578-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1578-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1578-150">Request body</span></span>

<span data-ttu-id="d1578-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1578-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1578-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1578-152">Response</span></span>

<span data-ttu-id="d1578-153">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos userAccountInformation](../resources/useraccountinformation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1578-153">If successful, this method returns a `200 OK` response code and a collection of [userAccountInformation](../resources/useraccountinformation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1578-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d1578-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d1578-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1578-155">Request</span></span>

<span data-ttu-id="d1578-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1578-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_account"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/account
```


### <a name="response"></a><span data-ttu-id="d1578-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1578-157">Response</span></span>

<span data-ttu-id="d1578-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d1578-158">The following is an example of the response.</span></span>

> <span data-ttu-id="d1578-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d1578-159">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation",
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
      "ageGroup": "adult",
      "countryCode": "NO",
      "preferredLanguageTag": null,
      "userPrincipalName": "innocenty.popov@adventureworks.com"
    }
  ]
}
```


