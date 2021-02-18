---
title: Listar responsabilidades
description: Obter as personResponsibilities da propriedade de navegação de responsabilidades.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c94ea1d4ef1e7014841b71876c927ce6fca952af
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292060"
---
# <a name="list-responsibilities"></a><span data-ttu-id="10b0d-103">Listar responsabilidades</span><span class="sxs-lookup"><span data-stu-id="10b0d-103">List responsibilities</span></span>
<span data-ttu-id="10b0d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10b0d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="10b0d-105">Recupere uma lista de [objetos personResponsibility](../resources/personresponsibility.md) do perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="10b0d-105">Retrieve a list of [personResponsibility](../resources/personresponsibility.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="10b0d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="10b0d-106">Permissions</span></span>

<span data-ttu-id="10b0d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10b0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10b0d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10b0d-109">Permission type</span></span>                        | <span data-ttu-id="10b0d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="10b0d-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="10b0d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10b0d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="10b0d-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10b0d-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="10b0d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10b0d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10b0d-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10b0d-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="10b0d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10b0d-115">Application</span></span>                            | <span data-ttu-id="10b0d-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10b0d-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="10b0d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10b0d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/responsibilities
GET /users/{id | userPrincipalName}/responsibilities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10b0d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="10b0d-118">Optional query parameters</span></span>

<span data-ttu-id="10b0d-119">Esse método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="10b0d-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="10b0d-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="10b0d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="10b0d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="10b0d-121">Name</span></span>            |<span data-ttu-id="10b0d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="10b0d-122">Value</span></span>    |<span data-ttu-id="10b0d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="10b0d-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="10b0d-124">$filter</span><span class="sxs-lookup"><span data-stu-id="10b0d-124">$filter</span></span>         |<span data-ttu-id="10b0d-125">string</span><span class="sxs-lookup"><span data-stu-id="10b0d-125">string</span></span>   |<span data-ttu-id="10b0d-126">Limita a resposta apenas aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="10b0d-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="10b0d-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="10b0d-127">$orderby</span></span>        |<span data-ttu-id="10b0d-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10b0d-128">string</span></span>   |<span data-ttu-id="10b0d-129">Por padrão, os objetos na resposta são organizados pelo valor createdDateTime em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="10b0d-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="10b0d-130">Você pode alterar a ordem da resposta usando o *$orderby* parâmetro.</span><span class="sxs-lookup"><span data-stu-id="10b0d-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="10b0d-131">$select</span><span class="sxs-lookup"><span data-stu-id="10b0d-131">$select</span></span>         |<span data-ttu-id="10b0d-132">string</span><span class="sxs-lookup"><span data-stu-id="10b0d-132">string</span></span>   |<span data-ttu-id="10b0d-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="10b0d-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="10b0d-135">$skip</span><span class="sxs-lookup"><span data-stu-id="10b0d-135">$skip</span></span>           |<span data-ttu-id="10b0d-136">int</span><span class="sxs-lookup"><span data-stu-id="10b0d-136">int</span></span>      |<span data-ttu-id="10b0d-137">Ignore os primeiros n resultados, útil para paging.</span><span class="sxs-lookup"><span data-stu-id="10b0d-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="10b0d-138">$top</span><span class="sxs-lookup"><span data-stu-id="10b0d-138">$top</span></span>            |<span data-ttu-id="10b0d-139">int</span><span class="sxs-lookup"><span data-stu-id="10b0d-139">int</span></span>      |<span data-ttu-id="10b0d-140">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="10b0d-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="10b0d-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10b0d-141">Request headers</span></span>
|<span data-ttu-id="10b0d-142">Nome</span><span class="sxs-lookup"><span data-stu-id="10b0d-142">Name</span></span>|<span data-ttu-id="10b0d-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="10b0d-143">Description</span></span>|
|:---|:---|
|<span data-ttu-id="10b0d-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="10b0d-144">Authorization</span></span>|<span data-ttu-id="10b0d-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10b0d-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="10b0d-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10b0d-147">Request body</span></span>
<span data-ttu-id="10b0d-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="10b0d-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10b0d-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="10b0d-149">Response</span></span>

<span data-ttu-id="10b0d-150">Se bem-sucedido, este método retorna um código de resposta e uma `200 OK` coleção de [objetos personResponsibility](../resources/personresponsibility.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10b0d-150">If successful, this method returns a `200 OK` response code and a collection of [personResponsibility](../resources/personresponsibility.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="10b0d-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="10b0d-151">Examples</span></span>

<!-- {
  "blockType": "request",
  "name": "get_responsibilities_from_profile"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/responsibilities
```

### <a name="response"></a><span data-ttu-id="10b0d-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="10b0d-152">Response</span></span>
<span data-ttu-id="10b0d-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="10b0d-153">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.personResponsibility)",
  "isCollection": true
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
      "description": "Member of the Microsoft API Council",
      "displayName": "API Council",
      "webUrl": null,
      "collaborationTags": [
        "askMeAbout"
      ]
    }
  ]
}
```


