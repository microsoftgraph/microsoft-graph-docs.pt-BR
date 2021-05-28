---
title: Instalar o aplicativo para o usuário
description: Instale um aplicativo no escopo pessoal do usuário especificado.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9a39bc198e742f2b5b1b15cbdbf02a96a980c708
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696279"
---
# <a name="install-app-for-user"></a><span data-ttu-id="0e334-103">Instalar o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="0e334-103">Install app for user</span></span>

<span data-ttu-id="0e334-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e334-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e334-105">Instale um [aplicativo](../resources/teamsapp.md) no escopo pessoal do usuário [especificado.](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="0e334-105">Install an [app](../resources/teamsapp.md) in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0e334-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e334-106">Permissions</span></span>

<span data-ttu-id="0e334-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e334-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e334-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e334-109">Permission type</span></span>      | <span data-ttu-id="0e334-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e334-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e334-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e334-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0e334-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="0e334-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="0e334-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e334-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e334-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e334-114">Not supported.</span></span>    |
|<span data-ttu-id="0e334-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e334-115">Application</span></span> | <span data-ttu-id="0e334-116">TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span><span class="sxs-lookup"><span data-stu-id="0e334-116">TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e334-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e334-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{user-id | user-principal-name}/teamwork/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="0e334-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e334-118">Request headers</span></span>

| <span data-ttu-id="0e334-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0e334-119">Header</span></span>       | <span data-ttu-id="0e334-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0e334-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0e334-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e334-121">Authorization</span></span>  | <span data-ttu-id="0e334-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e334-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0e334-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e334-124">Request body</span></span>

<span data-ttu-id="0e334-125">O corpo da solicitação deve conter a ID do aplicativo de catálogo existente a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="0e334-125">The request body should contain the ID of the existing catalog app to be added.</span></span>

| <span data-ttu-id="0e334-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e334-126">Property</span></span>   | <span data-ttu-id="0e334-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e334-127">Type</span></span> |<span data-ttu-id="0e334-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e334-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e334-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0e334-129">teamsApp</span></span>|<span data-ttu-id="0e334-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e334-130">String</span></span>|<span data-ttu-id="0e334-131">A ID do aplicativo a ser acrescentado.</span><span class="sxs-lookup"><span data-stu-id="0e334-131">The ID of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="0e334-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e334-132">Response</span></span>

<span data-ttu-id="0e334-p103">Se bem-sucedido, este método retorna um código de resposta `201 Created`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e334-p103">If successful, this method returns a `201 Created` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e334-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e334-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e334-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e334-136">Request</span></span>

<span data-ttu-id="0e334-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e334-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0e334-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e334-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_add_teamsApp"
}-->
```http
POST https://graph.microsoft.com/beta/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="c"></a>[<span data-ttu-id="0e334-139">C#</span><span class="sxs-lookup"><span data-stu-id="0e334-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-add-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e334-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e334-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-add-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e334-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e334-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-add-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e334-142">Java</span><span class="sxs-lookup"><span data-stu-id="0e334-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-add-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0e334-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e334-143">Response</span></span>

<span data-ttu-id="0e334-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0e334-144">The following is an example of the response.</span></span>

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


