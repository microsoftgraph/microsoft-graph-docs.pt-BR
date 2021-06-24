---
title: Obter userInsightsSettings
description: Recupere as propriedades de um objeto userInsightsSettings.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 11796934c9ea2edd7a5c3905604671f29604f973
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109059"
---
# <a name="get-userinsightssettings"></a><span data-ttu-id="a67e3-103">Obter userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="a67e3-103">Get userInsightsSettings</span></span>

<span data-ttu-id="a67e3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a67e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a67e3-105">Obter as configurações de privacidade personalizáveis pelo usuário [para o itemInsights](../resources/iteminsights.md) e informações do horário [de reunião.](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1)</span><span class="sxs-lookup"><span data-stu-id="a67e3-105">Get the user-customizable privacy settings for [itemInsights](../resources/iteminsights.md) and [meeting hours insights](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1).</span></span>

## <a name="permissions"></a><span data-ttu-id="a67e3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a67e3-106">Permissions</span></span>

<span data-ttu-id="a67e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a67e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a67e3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a67e3-109">Permission type</span></span>      | <span data-ttu-id="a67e3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a67e3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a67e3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a67e3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a67e3-112">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a67e3-112">User.Read, User.ReadWrite</span></span> |
|<span data-ttu-id="a67e3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a67e3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a67e3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a67e3-114">Not supported.</span></span>    |
|<span data-ttu-id="a67e3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a67e3-115">Application</span></span> | <span data-ttu-id="a67e3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a67e3-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="a67e3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a67e3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/settings/itemInsights
GET /user/{userId}/settings/itemInsights
```

><span data-ttu-id="a67e3-118">**Observação:** As solicitações com um ou são acessíveis apenas pelo usuário ou por um usuário com as permissões `userId` `userPrincipalName` User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="a67e3-118">**Note:** Requests with a `userId` or `userPrincipalName` are only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="a67e3-119">Para saber mais, confira [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a67e3-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a67e3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a67e3-120">Request headers</span></span>

| <span data-ttu-id="a67e3-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a67e3-121">Name</span></span>       | <span data-ttu-id="a67e3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a67e3-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="a67e3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a67e3-123">Authorization</span></span>  | <span data-ttu-id="a67e3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a67e3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a67e3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a67e3-126">Request body</span></span>

<span data-ttu-id="a67e3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a67e3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a67e3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a67e3-128">Response</span></span>

<span data-ttu-id="a67e3-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userInsightsSettings](../resources/userinsightssettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a67e3-129">If successful, this method returns a `200 OK` response code and a [userInsightsSettings](../resources/userinsightssettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a67e3-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a67e3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a67e3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a67e3-131">Request</span></span>

<span data-ttu-id="a67e3-132">A seguir, um exemplo da solicitação para obter informações de item do usuário e configurações de insights de horários de reunião.</span><span class="sxs-lookup"><span data-stu-id="a67e3-132">The following is an example of the request to get user item insights and meeting hours insights settings.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userInsightsSettings"
}-->

```http
GET https://graph.microsoft.com/beta/me/settings/itemInsights
```


### <a name="response"></a><span data-ttu-id="a67e3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a67e3-133">Response</span></span>

<span data-ttu-id="a67e3-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a67e3-134">The following is an example of the response.</span></span> 
> <span data-ttu-id="a67e3-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a67e3-135">**Note:** The response object shown here might be shortened for readability.</span></span>

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


