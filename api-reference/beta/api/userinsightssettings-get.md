---
title: Obter userInsightsSettings
description: Recupere as propriedades de um objeto userInsightsSettings.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: d3d9f370318f74f3c25b8737de4cecc7dbb37d6d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210338"
---
# <a name="get-userinsightssettings"></a><span data-ttu-id="7b123-103">Obter userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="7b123-103">Get userInsightsSettings</span></span>

<span data-ttu-id="7b123-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b123-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b123-105">Obter as configurações de privacidade personalizáveis pelo usuário [para o itemInsights](../resources/iteminsights.md) e informações do horário [de reunião.](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1)</span><span class="sxs-lookup"><span data-stu-id="7b123-105">Get the user-customizable privacy settings for [itemInsights](../resources/iteminsights.md) and [meeting hours insights](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1).</span></span>

## <a name="permissions"></a><span data-ttu-id="7b123-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7b123-106">Permissions</span></span>

<span data-ttu-id="7b123-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b123-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b123-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b123-109">Permission type</span></span>      | <span data-ttu-id="7b123-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b123-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b123-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b123-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7b123-112">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7b123-112">User.Read, User.ReadWrite</span></span> |
|<span data-ttu-id="7b123-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b123-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b123-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b123-114">Not supported.</span></span>    |
|<span data-ttu-id="7b123-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b123-115">Application</span></span> | <span data-ttu-id="7b123-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b123-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="7b123-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b123-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/settings/itemInsights
GET /user/{userId}/settings/itemInsights
```

><span data-ttu-id="7b123-118">**Observação:** As solicitações com um ou são acessíveis apenas pelo usuário ou por um usuário com as permissões `userId` `userPrincipalName` User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="7b123-118">**Note:** Requests with a `userId` or `userPrincipalName` are only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="7b123-119">Para saber mais, confira [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b123-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b123-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b123-120">Request headers</span></span>

| <span data-ttu-id="7b123-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7b123-121">Name</span></span>       | <span data-ttu-id="7b123-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b123-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="7b123-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b123-123">Authorization</span></span>  | <span data-ttu-id="7b123-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b123-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b123-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b123-126">Request body</span></span>

<span data-ttu-id="7b123-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7b123-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b123-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b123-128">Response</span></span>

<span data-ttu-id="7b123-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userInsightsSettings](../resources/userinsightssettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b123-129">If successful, this method returns a `200 OK` response code and a [userInsightsSettings](../resources/userinsightssettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7b123-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7b123-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7b123-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b123-131">Request</span></span>

<span data-ttu-id="7b123-132">A seguir, um exemplo da solicitação para obter informações de item do usuário e configurações de insights de horários de reunião.</span><span class="sxs-lookup"><span data-stu-id="7b123-132">The following is an example of the request to get user item insights and meeting hours insights settings.</span></span>


# <a name="http"></a>[<span data-ttu-id="7b123-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b123-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userInsightsSettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/settings/itemInsights
```
# <a name="c"></a>[<span data-ttu-id="7b123-134">C#</span><span class="sxs-lookup"><span data-stu-id="7b123-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userinsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b123-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b123-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userinsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b123-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b123-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userinsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b123-137">Java</span><span class="sxs-lookup"><span data-stu-id="7b123-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userinsightssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7b123-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b123-138">Response</span></span>

<span data-ttu-id="7b123-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7b123-139">The following is an example of the response.</span></span> 
> <span data-ttu-id="7b123-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7b123-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userInsightsSettings",
  "name": "get_userInsightsSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabled": true
}
```


