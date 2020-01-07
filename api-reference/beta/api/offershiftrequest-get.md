---
title: Obter offerShiftRequest
description: Recupere as propriedades e os relacionamentos de um objeto offerShiftRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 48fa2dc104dc609192232a4f173b314134829fb5
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952150"
---
# <a name="get-offershiftrequest"></a><span data-ttu-id="03514-103">Obter offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="03514-103">Get offerShiftRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03514-104">Recupere as propriedades e os relacionamentos de um objeto [offerShiftRequest](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="03514-104">Retrieve the properties and relationships of an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="03514-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="03514-105">Permissions</span></span>

<span data-ttu-id="03514-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03514-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="03514-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03514-108">Permission type</span></span>                        | <span data-ttu-id="03514-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="03514-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="03514-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03514-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="03514-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03514-111">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="03514-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03514-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03514-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03514-113">Not supported.</span></span> |
| <span data-ttu-id="03514-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03514-114">Application</span></span>                            | <span data-ttu-id="03514-115">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="03514-115">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="03514-116">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="03514-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="03514-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03514-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="03514-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="03514-118">Optional query parameters</span></span>

<span data-ttu-id="03514-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="03514-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="03514-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="03514-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="03514-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03514-121">Request headers</span></span>

| <span data-ttu-id="03514-122">Nome</span><span class="sxs-lookup"><span data-stu-id="03514-122">Name</span></span>      |<span data-ttu-id="03514-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="03514-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="03514-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="03514-124">Authorization</span></span> | <span data-ttu-id="03514-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03514-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03514-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03514-127">Request body</span></span>

<span data-ttu-id="03514-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="03514-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03514-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="03514-129">Response</span></span>

<span data-ttu-id="03514-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [offerShiftRequest](../resources/offershiftrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03514-130">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="03514-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="03514-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="03514-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03514-132">Request</span></span>

<span data-ttu-id="03514-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="03514-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```http
GET https://graph.microsoft.com/beta/teams/schedule/offerShiftRequests
```

### <a name="response"></a><span data-ttu-id="03514-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="03514-134">Response</span></span>

<span data-ttu-id="03514-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="03514-135">The following is an example of the response.</span></span>

> <span data-ttu-id="03514-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03514-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
