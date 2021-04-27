---
title: Obter leakedCredentialsRiskEvent
description: Recupere as propriedades e as relações de um objeto leakedcredentialsriskevent.
localization_priority: Normal
doc_type: apiPageType
author: cloudhandler
ms.prod: identity-and-sign-in
ms.openlocfilehash: 63abf3f0f1fa4ec1ca7c63f9a8a6169b0c61a821
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049321"
---
# <a name="get-leakedcredentialsriskevent-deprecated"></a><span data-ttu-id="bde92-103">Obter leakedCredentialsRiskEvent (preterido)</span><span class="sxs-lookup"><span data-stu-id="bde92-103">Get leakedCredentialsRiskEvent (deprecated)</span></span>

<span data-ttu-id="bde92-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bde92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="bde92-105">A **API identityRiskEvents** está preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="bde92-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="bde92-106">Para obter detalhes, [consulte Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="bde92-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="bde92-107">Recupere as propriedades e as relações de um objeto leakedcredentialsriskevent.</span><span class="sxs-lookup"><span data-stu-id="bde92-107">Retrieve the properties and relationships of a leakedcredentialsriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bde92-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="bde92-108">Permissions</span></span>
<span data-ttu-id="bde92-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bde92-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bde92-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bde92-111">Permission type</span></span>      | <span data-ttu-id="bde92-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bde92-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bde92-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bde92-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bde92-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="bde92-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="bde92-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bde92-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bde92-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bde92-116">Not supported.</span></span>    |
|<span data-ttu-id="bde92-117">Application</span><span class="sxs-lookup"><span data-stu-id="bde92-117">Application</span></span> | <span data-ttu-id="bde92-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="bde92-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bde92-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bde92-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bde92-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bde92-120">Request headers</span></span>
| <span data-ttu-id="bde92-121">Nome</span><span class="sxs-lookup"><span data-stu-id="bde92-121">Name</span></span>      |<span data-ttu-id="bde92-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bde92-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bde92-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bde92-123">Authorization</span></span>  | <span data-ttu-id="bde92-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bde92-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bde92-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bde92-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="bde92-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="bde92-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bde92-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bde92-129">Request body</span></span>
<span data-ttu-id="bde92-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bde92-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bde92-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="bde92-131">Response</span></span>

<span data-ttu-id="bde92-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bde92-132">If successful, this method returns a `200 OK` response code and [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bde92-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bde92-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bde92-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bde92-134">Request</span></span>
<span data-ttu-id="bde92-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bde92-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents/8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182
```
##### <a name="response"></a><span data-ttu-id="bde92-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bde92-136">Response</span></span>
<span data-ttu-id="bde92-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bde92-137">Here is an example of the response.</span></span> <span data-ttu-id="bde92-138">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bde92-138">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "closedDateTime": null,
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "active",
  "riskLevel": "high",
  "riskType": "LeakedCredentialsRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "278dc452-4163-dbc6-84eb-a050c37fc931",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get leakedCredentialsRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


