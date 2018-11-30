---
title: Obter riskyUsers
description: Recupere as propriedades e relacionamentos de um objeto **riskyUsers** .
ms.openlocfilehash: f0a6ac24bf66184d0547e9284f5a35b84b9358b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034130"
---
# <a name="get-riskyusers"></a><span data-ttu-id="ce4bd-103">Obter riskyUsers</span><span class="sxs-lookup"><span data-stu-id="ce4bd-103">Get riskyUsers</span></span>

> <span data-ttu-id="ce4bd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ce4bd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce4bd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ce4bd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ce4bd-106">Recupere as propriedades e relacionamentos de um objeto **riskyUsers** .</span><span class="sxs-lookup"><span data-stu-id="ce4bd-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ce4bd-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="ce4bd-107">Permissions</span></span>
<span data-ttu-id="ce4bd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce4bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce4bd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce4bd-110">Permission type</span></span>      | <span data-ttu-id="ce4bd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce4bd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce4bd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce4bd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ce4bd-113">IdentityrRskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce4bd-113">IdentityrRskyUser.Read.All</span></span>    |
|<span data-ttu-id="ce4bd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce4bd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce4bd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce4bd-115">Not supported.</span></span>    |
|<span data-ttu-id="ce4bd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce4bd-116">Application</span></span> | <span data-ttu-id="ce4bd-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce4bd-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce4bd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce4bd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="ce4bd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce4bd-119">Request headers</span></span>
| <span data-ttu-id="ce4bd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ce4bd-120">Name</span></span>      |<span data-ttu-id="ce4bd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce4bd-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ce4bd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce4bd-122">Authorization</span></span>  | <span data-ttu-id="ce4bd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce4bd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ce4bd-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ce4bd-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ce4bd-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ce4bd-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce4bd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce4bd-128">Request body</span></span>
<span data-ttu-id="ce4bd-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ce4bd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce4bd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce4bd-130">Response</span></span>

<span data-ttu-id="ce4bd-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [riskyUser](../resources/riskyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce4bd-131">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ce4bd-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce4bd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce4bd-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce4bd-133">Request</span></span>
<span data-ttu-id="ce4bd-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce4bd-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/{id}
```
##### <a name="response"></a><span data-ttu-id="ce4bd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce4bd-135">Response</span></span>
<span data-ttu-id="ce4bd-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce4bd-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 200 OK
{
  "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "riskLastUpdatedDateTime": "2016-01-29T20:03:57.7872426Z",
  "isGuest": "true",
  "isDeleted": "true",
  "riskDetail": "adminConfirmedSigninCompromised",
  "riskLevel": "high",
  "riskState": "atRisk"
  "userDisplayName": "Jon Doe",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
