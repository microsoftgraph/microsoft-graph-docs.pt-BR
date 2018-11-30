---
title: Lista unfamiliarLocationRiskEvents
description: Recupere uma lista de objetos unfamiliarlocationriskevent.
ms.openlocfilehash: 2a0decd6ecf700f2679bc905a7a64c261b7a532b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038247"
---
# <a name="list-unfamiliarlocationriskevents"></a><span data-ttu-id="5ca42-103">Lista unfamiliarLocationRiskEvents</span><span class="sxs-lookup"><span data-stu-id="5ca42-103">List unfamiliarLocationRiskEvents</span></span>

> <span data-ttu-id="5ca42-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5ca42-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ca42-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5ca42-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5ca42-106">Recupere uma lista de objetos unfamiliarlocationriskevent.</span><span class="sxs-lookup"><span data-stu-id="5ca42-106">Retrieve a list of unfamiliarlocationriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="5ca42-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="5ca42-107">Permissions</span></span>
<span data-ttu-id="5ca42-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ca42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ca42-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ca42-110">Permission type</span></span>      | <span data-ttu-id="5ca42-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ca42-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ca42-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ca42-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5ca42-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ca42-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="5ca42-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ca42-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ca42-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ca42-115">Not supported.</span></span>    |
|<span data-ttu-id="5ca42-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ca42-116">Application</span></span> | <span data-ttu-id="5ca42-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ca42-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ca42-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ca42-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /unfamiliarLocationRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="5ca42-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca42-119">Request headers</span></span>
| <span data-ttu-id="5ca42-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5ca42-120">Name</span></span>      |<span data-ttu-id="5ca42-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ca42-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5ca42-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ca42-122">Authorization</span></span>  | <span data-ttu-id="5ca42-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ca42-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5ca42-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5ca42-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="5ca42-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="5ca42-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ca42-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca42-128">Request body</span></span>
<span data-ttu-id="5ca42-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ca42-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ca42-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ca42-130">Response</span></span>

<span data-ttu-id="5ca42-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ca42-131">If successful, this method returns a `200 OK` response code and collection of [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5ca42-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ca42-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ca42-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca42-133">Request</span></span>
<span data-ttu-id="5ca42-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ca42-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unfamiliarlocationriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/unfamiliarLocationRiskEvents
```
##### <a name="response"></a><span data-ttu-id="5ca42-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ca42-135">Response</span></span>
<span data-ttu-id="5ca42-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ca42-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 290

{
  "value": [
    {
      "closedDateTime": "2016-01-29T20:03:57.7872426Z",
      "createdDateTime": "2016-01-29T00:01:49.126468Z",
      "id": "700b6476-8138-4c14-4962-c43614958301-8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad-4e5591fd-2ac1-4e9d-96a9-aca8339e2604",
      "ipAddress": "176.10.104.240",
      "location": "Bern, CH",
      "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
      "riskEventStatus": "remediated",
      "riskLevel": "medium",
      "riskType": "UnfamiliarLocationRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad",
      "userPrincipalName": "jon@contoso.com"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List unfamiliarLocationRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
