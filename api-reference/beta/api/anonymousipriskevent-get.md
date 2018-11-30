---
title: Obter anonymousIpRiskEvent
description: Recupere as propriedades e relacionamentos de um objeto anonymousipriskevent.
ms.openlocfilehash: 0dbc53f53ed029939cc02454041b63e6360d83c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034647"
---
# <a name="get-anonymousipriskevent"></a><span data-ttu-id="ace94-103">Obter anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ace94-103">Get anonymousIpRiskEvent</span></span>

> <span data-ttu-id="ace94-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ace94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ace94-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ace94-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ace94-106">Recupere as propriedades e relacionamentos de um objeto anonymousipriskevent.</span><span class="sxs-lookup"><span data-stu-id="ace94-106">Retrieve the properties and relationships of an anonymousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ace94-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="ace94-107">Permissions</span></span>
<span data-ttu-id="ace94-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ace94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ace94-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ace94-110">Permission type</span></span>      | <span data-ttu-id="ace94-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ace94-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ace94-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ace94-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ace94-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="ace94-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="ace94-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ace94-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ace94-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ace94-115">Not supported.</span></span>    |
|<span data-ttu-id="ace94-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ace94-116">Application</span></span> | <span data-ttu-id="ace94-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="ace94-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ace94-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ace94-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ace94-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ace94-119">Request headers</span></span>
| <span data-ttu-id="ace94-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ace94-120">Name</span></span>      |<span data-ttu-id="ace94-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ace94-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ace94-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ace94-122">Authorization</span></span>  | <span data-ttu-id="ace94-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ace94-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ace94-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ace94-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ace94-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ace94-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ace94-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ace94-128">Request body</span></span>
<span data-ttu-id="ace94-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ace94-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ace94-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ace94-130">Response</span></span>

<span data-ttu-id="ace94-131">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) no valor do corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ace94-131">If successful, this method returns a `200 OK` response code and [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object in the value of response body.</span></span>
## <a name="example"></a><span data-ttu-id="ace94-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ace94-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ace94-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ace94-133">Request</span></span>
<span data-ttu-id="ace94-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ace94-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents/2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71
```
##### <a name="response"></a><span data-ttu-id="ace94-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ace94-135">Response</span></span>
<span data-ttu-id="ace94-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ace94-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71",
  "ipAddress": null,
  "location": null,
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "AnonymousIpRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "6a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get anonymousIpRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
