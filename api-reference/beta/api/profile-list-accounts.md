---
title: Listar contas
description: Recupere uma lista de objetos userAccountInformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 44727e74b249828124413c120eb458cd0fd2b5a6
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292431"
---
# <a name="list-accounts"></a><span data-ttu-id="83b2c-103">Listar contas</span><span class="sxs-lookup"><span data-stu-id="83b2c-103">List accounts</span></span>

<span data-ttu-id="83b2c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83b2c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83b2c-105">Recupera propriedades relacionadas às contas do usuário do [perfil.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="83b2c-105">Retrieves properties related to the user's accounts from the [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="83b2c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="83b2c-106">Permissions</span></span>

<span data-ttu-id="83b2c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83b2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83b2c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83b2c-109">Permission type</span></span>                        | <span data-ttu-id="83b2c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83b2c-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="83b2c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83b2c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="83b2c-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b2c-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="83b2c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83b2c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83b2c-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b2c-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="83b2c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83b2c-115">Application</span></span>                            | <span data-ttu-id="83b2c-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b2c-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="83b2c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83b2c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/account
GET /users/{id | userPrincipalName}/profile/account
```

## <a name="optional-query-parameters"></a><span data-ttu-id="83b2c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="83b2c-118">Optional query parameters</span></span>

<span data-ttu-id="83b2c-119">Esse método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="83b2c-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="83b2c-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="83b2c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="83b2c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="83b2c-121">Name</span></span>            |<span data-ttu-id="83b2c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="83b2c-122">Value</span></span>    |<span data-ttu-id="83b2c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="83b2c-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="83b2c-124">$filter</span><span class="sxs-lookup"><span data-stu-id="83b2c-124">$filter</span></span>         |<span data-ttu-id="83b2c-125">string</span><span class="sxs-lookup"><span data-stu-id="83b2c-125">string</span></span>   |<span data-ttu-id="83b2c-126">Limita a resposta apenas aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="83b2c-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="83b2c-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="83b2c-127">$orderby</span></span>        |<span data-ttu-id="83b2c-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83b2c-128">string</span></span>   |<span data-ttu-id="83b2c-129">Por padrão, os objetos na resposta são organizados pelo valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="83b2c-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="83b2c-130">Você pode alterar a ordem da resposta usando o *$orderby* parâmetro.</span><span class="sxs-lookup"><span data-stu-id="83b2c-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="83b2c-131">$select</span><span class="sxs-lookup"><span data-stu-id="83b2c-131">$select</span></span>         |<span data-ttu-id="83b2c-132">string</span><span class="sxs-lookup"><span data-stu-id="83b2c-132">string</span></span>   |<span data-ttu-id="83b2c-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="83b2c-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="83b2c-135">$skip</span><span class="sxs-lookup"><span data-stu-id="83b2c-135">$skip</span></span>           |<span data-ttu-id="83b2c-136">int</span><span class="sxs-lookup"><span data-stu-id="83b2c-136">int</span></span>      |<span data-ttu-id="83b2c-137">Ignore os primeiros n resultados, útil para paging.</span><span class="sxs-lookup"><span data-stu-id="83b2c-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="83b2c-138">$top</span><span class="sxs-lookup"><span data-stu-id="83b2c-138">$top</span></span>            |<span data-ttu-id="83b2c-139">int</span><span class="sxs-lookup"><span data-stu-id="83b2c-139">int</span></span>      |<span data-ttu-id="83b2c-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="83b2c-140">Number of results to be returned.</span></span>                                                                                                                                           |


## <a name="request-headers"></a><span data-ttu-id="83b2c-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83b2c-141">Request headers</span></span>

| <span data-ttu-id="83b2c-142">Nome</span><span class="sxs-lookup"><span data-stu-id="83b2c-142">Name</span></span>           |<span data-ttu-id="83b2c-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="83b2c-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="83b2c-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="83b2c-144">Authorization</span></span>  | <span data-ttu-id="83b2c-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83b2c-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="83b2c-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="83b2c-147">Content-Type</span></span>   | <span data-ttu-id="83b2c-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83b2c-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83b2c-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83b2c-150">Request body</span></span>

<span data-ttu-id="83b2c-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="83b2c-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83b2c-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="83b2c-152">Response</span></span>

<span data-ttu-id="83b2c-153">Se bem-sucedido, este método retorna um código de resposta e uma coleção de `200 OK` [objetos userAccountInformation](../resources/useraccountinformation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83b2c-153">If successful, this method returns a `200 OK` response code and a collection of [userAccountInformation](../resources/useraccountinformation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="83b2c-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="83b2c-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="83b2c-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83b2c-155">Request</span></span>

<span data-ttu-id="83b2c-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="83b2c-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_account"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/account
```


### <a name="response"></a><span data-ttu-id="83b2c-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="83b2c-157">Response</span></span>

<span data-ttu-id="83b2c-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="83b2c-158">The following is an example of the response.</span></span>

> <span data-ttu-id="83b2c-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83b2c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


