---
title: 'offerShiftRequest: aprovar'
description: Aprovar um objeto offershiftrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 72662c2077a24b9bb253f26e1a314165792c43d4
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952178"
---
# <a name="offershiftrequest-approve"></a><span data-ttu-id="56bdb-103">offerShiftRequest: aprovar</span><span class="sxs-lookup"><span data-stu-id="56bdb-103">offerShiftRequest: approve</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56bdb-104">Aprovar um objeto [offershiftrequest](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="56bdb-104">Approve an [offershiftrequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="56bdb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="56bdb-105">Permissions</span></span>

<span data-ttu-id="56bdb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56bdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="56bdb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56bdb-108">Permission type</span></span>                        | <span data-ttu-id="56bdb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56bdb-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="56bdb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56bdb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="56bdb-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56bdb-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="56bdb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56bdb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56bdb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56bdb-113">Not supported.</span></span> |
| <span data-ttu-id="56bdb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56bdb-114">Application</span></span>                            | <span data-ttu-id="56bdb-115">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="56bdb-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="56bdb-116">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="56bdb-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="56bdb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56bdb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/schedule/offerShiftRequests/approve
```

## <a name="request-headers"></a><span data-ttu-id="56bdb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56bdb-118">Request headers</span></span>

| <span data-ttu-id="56bdb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="56bdb-119">Name</span></span>          | <span data-ttu-id="56bdb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="56bdb-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="56bdb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="56bdb-121">Authorization</span></span> | <span data-ttu-id="56bdb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56bdb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="56bdb-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="56bdb-124">Content-type</span></span> | <span data-ttu-id="56bdb-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56bdb-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56bdb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56bdb-127">Request body</span></span>

<span data-ttu-id="56bdb-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56bdb-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="56bdb-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="56bdb-129">Parameter</span></span>    | <span data-ttu-id="56bdb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="56bdb-130">Type</span></span>        | <span data-ttu-id="56bdb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="56bdb-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="56bdb-132">mensagem</span><span class="sxs-lookup"><span data-stu-id="56bdb-132">message</span></span>|<span data-ttu-id="56bdb-133">String</span><span class="sxs-lookup"><span data-stu-id="56bdb-133">String</span></span>|<span data-ttu-id="56bdb-134">Mensagem personalizada enviada na aprovação.</span><span class="sxs-lookup"><span data-stu-id="56bdb-134">Custom message sent on approval.</span></span>|

## <a name="response"></a><span data-ttu-id="56bdb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="56bdb-135">Response</span></span>

<span data-ttu-id="56bdb-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56bdb-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="56bdb-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="56bdb-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="56bdb-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56bdb-139">Request</span></span>

<span data-ttu-id="56bdb-140">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="56bdb-140">The following example shows a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/schedule/offerShiftRequests/approve
Content-type: application/json

{
  "message": "Approved!"
}
```

### <a name="response"></a><span data-ttu-id="56bdb-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="56bdb-141">Response</span></span>

<span data-ttu-id="56bdb-142">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="56bdb-142">The following example shows the response.</span></span>
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
  "description": "offerShiftRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
