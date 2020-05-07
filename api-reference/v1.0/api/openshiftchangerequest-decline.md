---
title: 'openShiftChangeRequest: recusar'
description: Recusar um openShiftChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b6a734f4f75c0d385f0df95d9b203332757bfdda
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155058"
---
# <a name="openshiftchangerequest-decline"></a><span data-ttu-id="306b7-103">openShiftChangeRequest: recusar</span><span class="sxs-lookup"><span data-stu-id="306b7-103">openShiftChangeRequest: decline</span></span>

<span data-ttu-id="306b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="306b7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="306b7-105">Recusar um objeto [openShiftChangeRequest](../resources/openshiftchangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="306b7-105">Decline an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="306b7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="306b7-106">Permissions</span></span>

<span data-ttu-id="306b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="306b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="306b7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="306b7-109">Permission type</span></span>                        | <span data-ttu-id="306b7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="306b7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="306b7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="306b7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="306b7-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="306b7-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="306b7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="306b7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="306b7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="306b7-114">Not supported.</span></span> |
| <span data-ttu-id="306b7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="306b7-115">Application</span></span>                            | <span data-ttu-id="306b7-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="306b7-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="306b7-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="306b7-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="306b7-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="306b7-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="306b7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="306b7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="306b7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="306b7-120">Request headers</span></span>

| <span data-ttu-id="306b7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="306b7-121">Name</span></span>          | <span data-ttu-id="306b7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="306b7-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="306b7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="306b7-123">Authorization</span></span> | <span data-ttu-id="306b7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="306b7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="306b7-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="306b7-126">Content-type</span></span> | <span data-ttu-id="306b7-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="306b7-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="306b7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="306b7-129">Request body</span></span>

<span data-ttu-id="306b7-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="306b7-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="306b7-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="306b7-131">Parameter</span></span>    | <span data-ttu-id="306b7-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="306b7-132">Type</span></span>        | <span data-ttu-id="306b7-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="306b7-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="306b7-134">mensagem</span><span class="sxs-lookup"><span data-stu-id="306b7-134">message</span></span>|<span data-ttu-id="306b7-135">String</span><span class="sxs-lookup"><span data-stu-id="306b7-135">String</span></span>|<span data-ttu-id="306b7-136">Uma mensagem de recusa personalizada.</span><span class="sxs-lookup"><span data-stu-id="306b7-136">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="306b7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="306b7-137">Response</span></span>

<span data-ttu-id="306b7-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="306b7-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="306b7-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="306b7-140">Examples</span></span>

<span data-ttu-id="306b7-141">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="306b7-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="306b7-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="306b7-142">Request</span></span>

<span data-ttu-id="306b7-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="306b7-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="306b7-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="306b7-144">Response</span></span>

<span data-ttu-id="306b7-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="306b7-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShiftChangeRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
