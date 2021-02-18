---
title: Obter personResponsibility
description: Leia as propriedades e os relacionamentos de um objeto personResponsibility.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 244313cd23c3a5635d75d3af7242df138ce253a5
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292704"
---
# <a name="get-personresponsibility"></a><span data-ttu-id="85fd0-103">Obter personResponsibility</span><span class="sxs-lookup"><span data-stu-id="85fd0-103">Get personResponsibility</span></span>
<span data-ttu-id="85fd0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85fd0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85fd0-105">Leia as propriedades e os relacionamentos de [um objeto personResponsibility](../resources/personresponsibility.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="85fd0-105">Read the properties and relationships of a [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="85fd0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="85fd0-106">Permissions</span></span>

<span data-ttu-id="85fd0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85fd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85fd0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85fd0-109">Permission type</span></span>                        | <span data-ttu-id="85fd0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85fd0-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="85fd0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85fd0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="85fd0-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85fd0-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="85fd0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85fd0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85fd0-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85fd0-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="85fd0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85fd0-115">Application</span></span>                            | <span data-ttu-id="85fd0-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85fd0-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="85fd0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85fd0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/responsibilities/{id}
GET /users/{id | userPrincipalName}/responsibilities/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="85fd0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="85fd0-118">Optional query parameters</span></span>

<span data-ttu-id="85fd0-119">Esse método dá suporte `$select` ao parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="85fd0-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="85fd0-120">Especifique uma lista de propriedades para incluir na resposta, separando-as por vírgulas.</span><span class="sxs-lookup"><span data-stu-id="85fd0-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="85fd0-121">Para obter o desempenho ideal, selecione apenas o subconjunto das propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="85fd0-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85fd0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85fd0-122">Request headers</span></span>
|<span data-ttu-id="85fd0-123">Nome</span><span class="sxs-lookup"><span data-stu-id="85fd0-123">Name</span></span>|<span data-ttu-id="85fd0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="85fd0-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="85fd0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="85fd0-125">Authorization</span></span>|<span data-ttu-id="85fd0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85fd0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="85fd0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85fd0-128">Request body</span></span>
<span data-ttu-id="85fd0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="85fd0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85fd0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="85fd0-130">Response</span></span>

<span data-ttu-id="85fd0-131">Se bem-sucedido, este método retorna um código de resposta e um `200 OK` [objeto personResponsibility](../resources/personresponsibility.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85fd0-131">If successful, this method returns a `200 OK` response code and a [personResponsibility](../resources/personresponsibility.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="85fd0-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="85fd0-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="85fd0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85fd0-133">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f"],
  "name": "get_personresponsibility"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/responsibilities/0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f
```

### <a name="response"></a><span data-ttu-id="85fd0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="85fd0-134">Response</span></span>
<span data-ttu-id="85fd0-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="85fd0-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personResponsibility"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

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
```


