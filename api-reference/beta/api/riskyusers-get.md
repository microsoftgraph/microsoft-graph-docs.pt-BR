---
title: Obter riskyUsers
description: Recupere as propriedades e os relacionamentos de um objeto **riskyUsers** .
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b65135fcd1ad77304b98f18fa595154aee984910
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/30/2019
ms.locfileid: "31003710"
---
# <a name="get-riskyusers"></a><span data-ttu-id="47bfd-103">Obter riskyUsers</span><span class="sxs-lookup"><span data-stu-id="47bfd-103">Get riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47bfd-104">Recupere as propriedades e os relacionamentos de um objeto **riskyUsers** .</span><span class="sxs-lookup"><span data-stu-id="47bfd-104">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

><span data-ttu-id="47bfd-105">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="47bfd-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="47bfd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="47bfd-106">Permissions</span></span>
<span data-ttu-id="47bfd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47bfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47bfd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47bfd-109">Permission type</span></span>      | <span data-ttu-id="47bfd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47bfd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47bfd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47bfd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="47bfd-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="47bfd-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="47bfd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47bfd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47bfd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47bfd-114">Not supported.</span></span>    |
|<span data-ttu-id="47bfd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47bfd-115">Application</span></span> | <span data-ttu-id="47bfd-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="47bfd-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47bfd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47bfd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="47bfd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47bfd-118">Request headers</span></span>
| <span data-ttu-id="47bfd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="47bfd-119">Name</span></span>      |<span data-ttu-id="47bfd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="47bfd-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="47bfd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="47bfd-121">Authorization</span></span>  | <span data-ttu-id="47bfd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47bfd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="47bfd-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="47bfd-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="47bfd-125">ID da sessão da pasta de trabalho que determina se as alterações são persistentes.</span><span class="sxs-lookup"><span data-stu-id="47bfd-125">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="47bfd-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="47bfd-126">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47bfd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47bfd-127">Request body</span></span>
<span data-ttu-id="47bfd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47bfd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47bfd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="47bfd-129">Response</span></span>

<span data-ttu-id="47bfd-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [riskyUser](../resources/riskyUser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47bfd-130">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyUser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="47bfd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47bfd-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47bfd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47bfd-132">Request</span></span>
<span data-ttu-id="47bfd-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47bfd-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/{id}
```
##### <a name="response"></a><span data-ttu-id="47bfd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="47bfd-134">Response</span></span>
<span data-ttu-id="47bfd-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47bfd-135">Here is an example of the response.</span></span>
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
  "isProcessing": true,
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

