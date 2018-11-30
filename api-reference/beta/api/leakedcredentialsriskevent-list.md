---
title: Lista leakedCredentialsRiskEvents
description: Recupere uma lista de objetos leakedcredentialsriskevent.
ms.openlocfilehash: 49cfd54c580634e43cff50aa7c125ffc79116ea3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038317"
---
# <a name="list-leakedcredentialsriskevents"></a><span data-ttu-id="76f96-103">Lista leakedCredentialsRiskEvents</span><span class="sxs-lookup"><span data-stu-id="76f96-103">List leakedCredentialsRiskEvents</span></span>

> <span data-ttu-id="76f96-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="76f96-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76f96-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="76f96-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76f96-106">Recupere uma lista de objetos leakedcredentialsriskevent.</span><span class="sxs-lookup"><span data-stu-id="76f96-106">Retrieve a list of leakedcredentialsriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="76f96-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="76f96-107">Permissions</span></span>
<span data-ttu-id="76f96-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76f96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76f96-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76f96-110">Permission type</span></span>      | <span data-ttu-id="76f96-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76f96-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76f96-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76f96-112">Delegated (work or school account)</span></span> | <span data-ttu-id="76f96-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="76f96-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="76f96-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76f96-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76f96-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76f96-115">Not supported.</span></span>    |
|<span data-ttu-id="76f96-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76f96-116">Application</span></span> | <span data-ttu-id="76f96-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="76f96-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76f96-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76f96-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="76f96-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76f96-119">Request headers</span></span>
| <span data-ttu-id="76f96-120">Nome</span><span class="sxs-lookup"><span data-stu-id="76f96-120">Name</span></span>      |<span data-ttu-id="76f96-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="76f96-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="76f96-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="76f96-122">Authorization</span></span>  | <span data-ttu-id="76f96-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76f96-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="76f96-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="76f96-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="76f96-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="76f96-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="76f96-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76f96-128">Request body</span></span>
<span data-ttu-id="76f96-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="76f96-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76f96-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="76f96-130">Response</span></span>

<span data-ttu-id="76f96-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76f96-131">If successful, this method returns a `200 OK` response code and collection of [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="76f96-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76f96-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76f96-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76f96-133">Request</span></span>
<span data-ttu-id="76f96-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76f96-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents
```
##### <a name="response"></a><span data-ttu-id="76f96-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="76f96-135">Response</span></span>
<span data-ttu-id="76f96-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76f96-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List leakedCredentialsRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
