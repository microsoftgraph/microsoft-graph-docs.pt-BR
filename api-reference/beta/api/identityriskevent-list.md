---
title: Lista identityRiskEvents
description: Recupere uma lista de objetos identityriskevent.
author: cloudhandler
ms.openlocfilehash: ee730b2da90cd1d458bd3e3ad4c432db93fa4cea
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302776"
---
# <a name="list-identityriskevents"></a><span data-ttu-id="4bf1c-103">Lista identityRiskEvents</span><span class="sxs-lookup"><span data-stu-id="4bf1c-103">List identityRiskEvents</span></span>

> <span data-ttu-id="4bf1c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4bf1c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4bf1c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4bf1c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4bf1c-106">Recupere uma lista de objetos identityriskevent.</span><span class="sxs-lookup"><span data-stu-id="4bf1c-106">Retrieve a list of identityriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="4bf1c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4bf1c-107">Permissions</span></span>
<span data-ttu-id="4bf1c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bf1c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bf1c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4bf1c-110">Permission type</span></span>      | <span data-ttu-id="4bf1c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4bf1c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bf1c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4bf1c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4bf1c-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bf1c-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="4bf1c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4bf1c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bf1c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bf1c-115">Not supported.</span></span>    |
|<span data-ttu-id="4bf1c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bf1c-116">Application</span></span> | <span data-ttu-id="4bf1c-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bf1c-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bf1c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4bf1c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="4bf1c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4bf1c-119">Request headers</span></span>
| <span data-ttu-id="4bf1c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4bf1c-120">Name</span></span>      |<span data-ttu-id="4bf1c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bf1c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4bf1c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4bf1c-122">Authorization</span></span>  | <span data-ttu-id="4bf1c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4bf1c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4bf1c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4bf1c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="4bf1c-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="4bf1c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bf1c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4bf1c-128">Request body</span></span>
<span data-ttu-id="4bf1c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4bf1c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bf1c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bf1c-130">Response</span></span>

<span data-ttu-id="4bf1c-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [identityRiskEvent](../resources/identityriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bf1c-131">If successful, this method returns a `200 OK` response code and collection of [identityRiskEvent](../resources/identityriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4bf1c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4bf1c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4bf1c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bf1c-133">Request</span></span>
<span data-ttu-id="4bf1c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bf1c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityRiskEvents
```
##### <a name="response"></a><span data-ttu-id="4bf1c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bf1c-135">Response</span></span>
<span data-ttu-id="4bf1c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4bf1c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.malwareRiskEvent",
      "malwareName": "CONFICKER",
      "closedDateTime": null,
      "createdDateTime": "2016-02-03T06:06:01.940814Z",
      "deviceInformation": "B62XYZ13OX",
      "id": "74ceb0af-2271-9167-ffa0-b6ac3b4e8781-9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89-0fdc2304-ba4c-ac0c-bdd7-da2d10e93849",
      "ipAddress": "95.31.18.119",
      "location": "Moskva, Russia, RU",
      "riskEventDateTime": "2016-02-03T05:20:33.7208156Z",
      "riskEventStatus": "active",
      "riskLevel": "low",
      "riskType": "MalwareRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89",
      "userPrincipalName": "jon@contoso.com"
    },
    {
      "@odata.type": "#microsoft.graph.unfamiliarLocationRiskEvent",
      "closedDateTime": "2016-01-29T20:03:57.7872426Z",
      "createdDateTime": "2016-01-29T00:01:49.126468Z",
      "id": "ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89-db69711e-9324-ec99-f010-6e63fb972e98",
      "ipAddress": "176.10.104.240",
      "location": "Bern, CH",
      "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
      "riskEventStatus": "remediated",
      "riskLevel": "medium",
      "riskType": "UnfamiliarLocationRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89",
      "userPrincipalName": "jon@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List identityRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
