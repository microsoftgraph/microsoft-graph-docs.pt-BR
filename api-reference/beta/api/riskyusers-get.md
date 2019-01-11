---
title: Obter riskyUsers
description: Recupere as propriedades e relacionamentos de um objeto **riskyUsers** .
localization_priority: Normal
ms.openlocfilehash: da26be10b5a1aa631bd55f977ead806ed89c1406
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891123"
---
# <a name="get-riskyusers"></a><span data-ttu-id="1f900-103">Obter riskyUsers</span><span class="sxs-lookup"><span data-stu-id="1f900-103">Get riskyUsers</span></span>

> <span data-ttu-id="1f900-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1f900-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f900-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1f900-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f900-106">Recupere as propriedades e relacionamentos de um objeto **riskyUsers** .</span><span class="sxs-lookup"><span data-stu-id="1f900-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="1f900-107">**Observação:** Esta API requer uma licença de P2 Premium do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1f900-107">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f900-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="1f900-108">Permissions</span></span>
<span data-ttu-id="1f900-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f900-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f900-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f900-111">Permission type</span></span>      | <span data-ttu-id="1f900-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f900-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f900-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f900-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1f900-114">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f900-114">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="1f900-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f900-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f900-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f900-116">Not supported.</span></span>    |
|<span data-ttu-id="1f900-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f900-117">Application</span></span> | <span data-ttu-id="1f900-118">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f900-118">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f900-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f900-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="1f900-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f900-120">Request headers</span></span>
| <span data-ttu-id="1f900-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1f900-121">Name</span></span>      |<span data-ttu-id="1f900-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f900-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1f900-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f900-123">Authorization</span></span>  | <span data-ttu-id="1f900-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f900-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1f900-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1f900-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="1f900-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1f900-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f900-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f900-129">Request body</span></span>
<span data-ttu-id="1f900-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1f900-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f900-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f900-131">Response</span></span>

<span data-ttu-id="1f900-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [riskyUser](../resources/riskyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f900-132">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f900-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f900-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f900-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f900-134">Request</span></span>
<span data-ttu-id="1f900-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f900-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/{id}
```
##### <a name="response"></a><span data-ttu-id="1f900-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f900-136">Response</span></span>
<span data-ttu-id="1f900-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f900-137">Here is an example of the response.</span></span>
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
