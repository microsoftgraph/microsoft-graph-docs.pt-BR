---
title: Listar offerShiftRequest
description: Recupere as propriedades e os relacionamentos de todos os objetos offerShiftRequest de uma equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9b2c722b3217395928fb6a60d29d6e43b6d36792
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154925"
---
# <a name="list-offershiftrequest"></a><span data-ttu-id="1b8b0-103">Listar offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="1b8b0-103">List offerShiftRequest</span></span>

<span data-ttu-id="1b8b0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b8b0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1b8b0-105">Recupere as propriedades e os relacionamentos de todos os objetos [offerShiftRequest](../resources/offershiftrequest.md) de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="1b8b0-105">Retrieve the properties and relationships of all [offerShiftRequest](../resources/offershiftrequest.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b8b0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b8b0-106">Permissions</span></span>

<span data-ttu-id="1b8b0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b8b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1b8b0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b8b0-109">Permission type</span></span>                        | <span data-ttu-id="1b8b0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b8b0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1b8b0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b8b0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1b8b0-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1b8b0-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1b8b0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b8b0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b8b0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b8b0-114">Not supported.</span></span> |
| <span data-ttu-id="1b8b0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b8b0-115">Application</span></span>                            | <span data-ttu-id="1b8b0-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b8b0-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="1b8b0-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="1b8b0-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1b8b0-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="1b8b0-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1b8b0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b8b0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1b8b0-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1b8b0-120">Optional query parameters</span></span>

<span data-ttu-id="1b8b0-121">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1b8b0-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1b8b0-122">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1b8b0-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b8b0-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b8b0-123">Request headers</span></span>

| <span data-ttu-id="1b8b0-124">Nome</span><span class="sxs-lookup"><span data-stu-id="1b8b0-124">Name</span></span>      |<span data-ttu-id="1b8b0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b8b0-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1b8b0-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b8b0-126">Authorization</span></span> | <span data-ttu-id="1b8b0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b8b0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b8b0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b8b0-129">Request body</span></span>

<span data-ttu-id="1b8b0-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1b8b0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b8b0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b8b0-131">Response</span></span>

<span data-ttu-id="1b8b0-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e os objetos [offerShiftRequest](../resources/offershiftrequest.md) solicitados no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b8b0-132">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b8b0-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1b8b0-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1b8b0-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b8b0-134">Request</span></span>

<span data-ttu-id="1b8b0-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b8b0-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests
```
---


### <a name="response"></a><span data-ttu-id="1b8b0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b8b0-136">Response</span></span>

<span data-ttu-id="1b8b0-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1b8b0-137">The following is an example of the response.</span></span>

> <span data-ttu-id="1b8b0-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b8b0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.offerShiftRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "recipientActionMessage": "recipientActionMessage-value",
  "recipientActionDateTime": "datetime-value",
  "senderShiftId": "senderShiftId-value",
  "recipientUserId": "recipientUserId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get offerShiftRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
