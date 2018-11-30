---
title: Obter leakedCredentialsRiskEvent
description: Recupere as propriedades e relacionamentos de um objeto leakedcredentialsriskevent.
ms.openlocfilehash: a3d259f785d2c8d6717f4dfe90ba04aeb454a1bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040519"
---
# <a name="get-leakedcredentialsriskevent"></a><span data-ttu-id="e3ec2-103">Obter leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e3ec2-103">Get leakedCredentialsRiskEvent</span></span>

> <span data-ttu-id="e3ec2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e3ec2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3ec2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e3ec2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3ec2-106">Recupere as propriedades e relacionamentos de um objeto leakedcredentialsriskevent.</span><span class="sxs-lookup"><span data-stu-id="e3ec2-106">Retrieve the properties and relationships of a leakedcredentialsriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e3ec2-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="e3ec2-107">Permissions</span></span>
<span data-ttu-id="e3ec2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3ec2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3ec2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3ec2-110">Permission type</span></span>      | <span data-ttu-id="e3ec2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3ec2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3ec2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3ec2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e3ec2-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3ec2-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="e3ec2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3ec2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3ec2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3ec2-115">Not supported.</span></span>    |
|<span data-ttu-id="e3ec2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3ec2-116">Application</span></span> | <span data-ttu-id="e3ec2-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3ec2-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3ec2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3ec2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e3ec2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3ec2-119">Request headers</span></span>
| <span data-ttu-id="e3ec2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e3ec2-120">Name</span></span>      |<span data-ttu-id="e3ec2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3ec2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e3ec2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3ec2-122">Authorization</span></span>  | <span data-ttu-id="e3ec2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3ec2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e3ec2-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e3ec2-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="e3ec2-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e3ec2-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3ec2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3ec2-128">Request body</span></span>
<span data-ttu-id="e3ec2-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e3ec2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3ec2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3ec2-130">Response</span></span>

<span data-ttu-id="e3ec2-131">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3ec2-131">If successful, this method returns a `200 OK` response code and [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e3ec2-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3ec2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3ec2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3ec2-133">Request</span></span>
<span data-ttu-id="e3ec2-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3ec2-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents/8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182
```
##### <a name="response"></a><span data-ttu-id="e3ec2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3ec2-135">Response</span></span>
<span data-ttu-id="e3ec2-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3ec2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get leakedCredentialsRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
