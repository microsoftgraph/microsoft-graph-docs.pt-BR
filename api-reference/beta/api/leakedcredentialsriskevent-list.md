---
title: Listar leakedCredentialsRiskEvents
description: Recupere uma lista de objetos leakedcredentialsriskevent.
localization_priority: Normal
doc_type: apiPageType
author: cloudhandler
ms.prod: identity-and-sign-in
ms.openlocfilehash: 0b27be914e14371c091ff4de7547f96e4d6c003b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443759"
---
# <a name="list-leakedcredentialsriskevents-deprecated"></a><span data-ttu-id="59649-103">Listar leakedCredentialsRiskEvents (preterido)</span><span class="sxs-lookup"><span data-stu-id="59649-103">List leakedCredentialsRiskEvents (deprecated)</span></span>

<span data-ttu-id="59649-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59649-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="59649-105">A **API identityRiskEvents** está preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="59649-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="59649-106">Para obter detalhes, [consulte Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="59649-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="59649-107">Recupere uma lista de objetos leakedcredentialsriskevent.</span><span class="sxs-lookup"><span data-stu-id="59649-107">Retrieve a list of leakedcredentialsriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="59649-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="59649-108">Permissions</span></span>
<span data-ttu-id="59649-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59649-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59649-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59649-111">Permission type</span></span>      | <span data-ttu-id="59649-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59649-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59649-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59649-113">Delegated (work or school account)</span></span> | <span data-ttu-id="59649-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="59649-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="59649-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59649-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59649-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59649-116">Not supported.</span></span>    |
|<span data-ttu-id="59649-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59649-117">Application</span></span> | <span data-ttu-id="59649-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="59649-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59649-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59649-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="59649-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59649-120">Request headers</span></span>
| <span data-ttu-id="59649-121">Nome</span><span class="sxs-lookup"><span data-stu-id="59649-121">Name</span></span>      |<span data-ttu-id="59649-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="59649-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="59649-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="59649-123">Authorization</span></span>  | <span data-ttu-id="59649-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59649-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59649-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="59649-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="59649-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="59649-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59649-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59649-129">Request body</span></span>
<span data-ttu-id="59649-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="59649-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59649-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="59649-131">Response</span></span>

<span data-ttu-id="59649-132">Se tiver êxito, este método retornará um código de resposta e `200 OK` uma coleção de objetos [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59649-132">If successful, this method returns a `200 OK` response code and collection of [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59649-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59649-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59649-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59649-134">Request</span></span>
<span data-ttu-id="59649-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59649-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents
```
##### <a name="response"></a><span data-ttu-id="59649-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="59649-136">Response</span></span>
<span data-ttu-id="59649-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59649-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "value":
  [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List leakedCredentialsRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


