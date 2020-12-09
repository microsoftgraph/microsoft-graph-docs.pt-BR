---
title: Instalar o aplicativo para o usuário
description: Instale um aplicativo no escopo pessoal do usuário especificado.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7699a91b2700d9c85843b51d78666d7b821c6150
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607311"
---
# <a name="install-app-for-user"></a><span data-ttu-id="7259f-103">Instalar o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="7259f-103">Install app for user</span></span>

<span data-ttu-id="7259f-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7259f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7259f-105">Instalar um [aplicativo](../resources/teamsapp.md) no escopo pessoal do [usuário](../resources/user.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="7259f-105">Install an [app](../resources/teamsapp.md) in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7259f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7259f-106">Permissions</span></span>

<span data-ttu-id="7259f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7259f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7259f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7259f-109">Permission type</span></span>      | <span data-ttu-id="7259f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7259f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7259f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7259f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7259f-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="7259f-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="7259f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7259f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7259f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7259f-114">Not supported.</span></span>    |
|<span data-ttu-id="7259f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7259f-115">Application</span></span> | <span data-ttu-id="7259f-116">TeamsAppInstallation. ReadWriteSelfForUser. All, TeamsAppInstallation. ReadWriteForUser. All</span><span class="sxs-lookup"><span data-stu-id="7259f-116">TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7259f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7259f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{user-id}/teamwork/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="7259f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7259f-118">Request headers</span></span>

| <span data-ttu-id="7259f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7259f-119">Header</span></span>       | <span data-ttu-id="7259f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="7259f-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7259f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7259f-121">Authorization</span></span>  | <span data-ttu-id="7259f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7259f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7259f-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="7259f-124">Content-type</span></span> | <span data-ttu-id="7259f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7259f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7259f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7259f-127">Request body</span></span>

<span data-ttu-id="7259f-128">O corpo da solicitação deve conter a ID do aplicativo de catálogo existente a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="7259f-128">The request body should contain the ID of the existing catalog app to be added.</span></span>

| <span data-ttu-id="7259f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7259f-129">Property</span></span>   | <span data-ttu-id="7259f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7259f-130">Type</span></span> |<span data-ttu-id="7259f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7259f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7259f-132">teamsApp</span><span class="sxs-lookup"><span data-stu-id="7259f-132">teamsApp</span></span>|<span data-ttu-id="7259f-133">String</span><span class="sxs-lookup"><span data-stu-id="7259f-133">String</span></span>|<span data-ttu-id="7259f-134">A ID do aplicativo a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="7259f-134">The ID of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="7259f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7259f-135">Response</span></span>

<span data-ttu-id="7259f-p104">Se bem-sucedido, este método retorna um código de resposta `201 Created`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7259f-p104">If successful, this method returns a `201 Created` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7259f-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7259f-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="7259f-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7259f-139">Request</span></span>

<span data-ttu-id="7259f-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7259f-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_add_teamsApp"
}-->

```http
POST https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```

### <a name="response"></a><span data-ttu-id="7259f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7259f-141">Response</span></span>
<span data-ttu-id="7259f-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7259f-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User add teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
