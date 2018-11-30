---
title: Obter unfamiliarLocationRiskEvent
description: Recupere as propriedades e relacionamentos de um objeto unfamiliarlocationriskevent.
ms.openlocfilehash: e75399b79b8f3535741549ce49f5cfcb5ee40077
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041168"
---
# <a name="get-unfamiliarlocationriskevent"></a><span data-ttu-id="34a38-103">Obter unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="34a38-103">Get unfamiliarLocationRiskEvent</span></span>

> <span data-ttu-id="34a38-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="34a38-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34a38-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="34a38-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34a38-106">Recupere as propriedades e relacionamentos de um objeto unfamiliarlocationriskevent.</span><span class="sxs-lookup"><span data-stu-id="34a38-106">Retrieve the properties and relationships of an unfamiliarlocationriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="34a38-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="34a38-107">Permissions</span></span>
<span data-ttu-id="34a38-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34a38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34a38-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34a38-110">Permission type</span></span>      | <span data-ttu-id="34a38-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34a38-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34a38-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34a38-112">Delegated (work or school account)</span></span> | <span data-ttu-id="34a38-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="34a38-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="34a38-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34a38-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34a38-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34a38-115">Not supported.</span></span>    |
|<span data-ttu-id="34a38-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34a38-116">Application</span></span> | <span data-ttu-id="34a38-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="34a38-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="34a38-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34a38-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /unfamiliarLocationRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="34a38-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34a38-119">Request headers</span></span>
| <span data-ttu-id="34a38-120">Nome</span><span class="sxs-lookup"><span data-stu-id="34a38-120">Name</span></span>      |<span data-ttu-id="34a38-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="34a38-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="34a38-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="34a38-122">Authorization</span></span>  | <span data-ttu-id="34a38-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34a38-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34a38-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="34a38-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="34a38-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="34a38-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="34a38-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34a38-128">Request body</span></span>
<span data-ttu-id="34a38-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34a38-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34a38-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="34a38-130">Response</span></span>

<span data-ttu-id="34a38-131">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34a38-131">If successful, this method returns a `200 OK` response code and [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="34a38-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34a38-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34a38-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34a38-133">Request</span></span>
<span data-ttu-id="34a38-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34a38-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unfamiliarlocationriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/unfamiliarLocationRiskEvents/700b6476-8138-4c14-4962-c43614958301-8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad-4e5591fd-2ac1-4e9d-96a9-aca8339e2604
```
##### <a name="response"></a><span data-ttu-id="34a38-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="34a38-135">Response</span></span>
<span data-ttu-id="34a38-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34a38-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unfamiliarLocationRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
