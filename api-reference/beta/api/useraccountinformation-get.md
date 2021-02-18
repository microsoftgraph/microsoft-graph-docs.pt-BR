---
title: Obter userAccountInformation
description: Recupere as propriedades e os relacionamentos do objeto userAccountInformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: Profile
doc_type: apiPageType
ms.openlocfilehash: c9418fad469cd831c2620f79408ff06266d69f3b
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291934"
---
# <a name="get-useraccountinformation"></a><span data-ttu-id="497a7-103">Obter userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="497a7-103">Get userAccountInformation</span></span>

<span data-ttu-id="497a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="497a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="497a7-105">Recupere as propriedades e os relacionamentos de [um objeto userAccountInformation](../resources/useraccountinformation.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="497a7-105">Retrieve the properties and relationships of an [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="497a7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="497a7-106">Permissions</span></span>

<span data-ttu-id="497a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="497a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="497a7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="497a7-109">Permission type</span></span>                        | <span data-ttu-id="497a7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="497a7-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="497a7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="497a7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="497a7-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="497a7-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="497a7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="497a7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="497a7-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="497a7-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="497a7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="497a7-115">Application</span></span>                            | <span data-ttu-id="497a7-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="497a7-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="497a7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="497a7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/account/{id}
GET /users/{id | userPrincipalName}/profile/account/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="497a7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="497a7-118">Optional query parameters</span></span>

<span data-ttu-id="497a7-119">Esse método dá suporte `$select` ao parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="497a7-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="497a7-120">Especifique uma lista de propriedades a incluir na resposta, separando-as por vírgulas.</span><span class="sxs-lookup"><span data-stu-id="497a7-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="497a7-121">Para obter o desempenho ideal, selecione apenas o subconjunto das propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="497a7-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="497a7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="497a7-122">Request headers</span></span>

| <span data-ttu-id="497a7-123">Nome</span><span class="sxs-lookup"><span data-stu-id="497a7-123">Name</span></span>          |<span data-ttu-id="497a7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="497a7-124">Description</span></span>                |
|:--------------|:--------------------------|
| <span data-ttu-id="497a7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="497a7-125">Authorization</span></span> | <span data-ttu-id="497a7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="497a7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="497a7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="497a7-128">Request body</span></span>

<span data-ttu-id="497a7-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="497a7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="497a7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="497a7-130">Response</span></span>

<span data-ttu-id="497a7-131">Se bem-sucedido, este método retorna um código de resposta e o objeto `200 OK` [userAccountInformation](../resources/useraccountinformation.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="497a7-131">If successful, this method returns a `200 OK` response code and the requested [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="497a7-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="497a7-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="497a7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="497a7-133">Request</span></span>

<span data-ttu-id="497a7-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="497a7-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_useraccountinformation"
}-->

```http
GET https://graph.microsoft.com/beta/me/profile/account/{id}
```

### <a name="response"></a><span data-ttu-id="497a7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="497a7-135">Response</span></span>

<span data-ttu-id="497a7-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="497a7-136">The following is an example of the response.</span></span>

> <span data-ttu-id="497a7-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="497a7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```


