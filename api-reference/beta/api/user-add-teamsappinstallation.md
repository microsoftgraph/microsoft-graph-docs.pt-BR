---
title: Instalar o aplicativo para o usuário
description: Instale um aplicativo no escopo pessoal do usuário especificado.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5eda35222f66f6ebb522e449cc1242c8e822f250
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976631"
---
# <a name="install-app-for-user"></a><span data-ttu-id="710fd-103">Instalar o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="710fd-103">Install app for user</span></span>

<span data-ttu-id="710fd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="710fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="710fd-105">Instalar um [aplicativo](../resources/teamsapp.md) no escopo pessoal do [usuário](../resources/user.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="710fd-105">Install an [app](../resources/teamsapp.md) in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="710fd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="710fd-106">Permissions</span></span>

<span data-ttu-id="710fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="710fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="710fd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="710fd-109">Permission type</span></span>      | <span data-ttu-id="710fd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="710fd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="710fd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="710fd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="710fd-112">TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="710fd-112">TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="710fd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="710fd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="710fd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="710fd-114">Not supported.</span></span>    |
|<span data-ttu-id="710fd-115">Application</span><span class="sxs-lookup"><span data-stu-id="710fd-115">Application</span></span> | <span data-ttu-id="710fd-116">TeamsAppInstallation.ReadWriteForUser.All</span><span class="sxs-lookup"><span data-stu-id="710fd-116">TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="710fd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="710fd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="710fd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="710fd-118">Request headers</span></span>

| <span data-ttu-id="710fd-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="710fd-119">Header</span></span>       | <span data-ttu-id="710fd-120">Valor</span><span class="sxs-lookup"><span data-stu-id="710fd-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="710fd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="710fd-121">Authorization</span></span>  | <span data-ttu-id="710fd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="710fd-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="710fd-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="710fd-124">Request body</span></span>

<span data-ttu-id="710fd-125">O corpo da solicitação deve conter a ID do aplicativo de catálogo existente a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="710fd-125">The request body should contain the ID of the existing catalog app to be added.</span></span>

| <span data-ttu-id="710fd-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="710fd-126">Property</span></span>   | <span data-ttu-id="710fd-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="710fd-127">Type</span></span> |<span data-ttu-id="710fd-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="710fd-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="710fd-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="710fd-129">teamsApp</span></span>|<span data-ttu-id="710fd-130">String</span><span class="sxs-lookup"><span data-stu-id="710fd-130">String</span></span>|<span data-ttu-id="710fd-131">A ID do aplicativo a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="710fd-131">The ID of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="710fd-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="710fd-132">Response</span></span>

<span data-ttu-id="710fd-p103">Se bem-sucedido, este método retorna um código de resposta `201 Created`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="710fd-p103">If successful, this method returns a `201 Created` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="710fd-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="710fd-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="710fd-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="710fd-136">Request</span></span>

<span data-ttu-id="710fd-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="710fd-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="710fd-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="710fd-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_add_teamsApp"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="c"></a>[<span data-ttu-id="710fd-139">C#</span><span class="sxs-lookup"><span data-stu-id="710fd-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-add-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="710fd-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="710fd-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-add-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="710fd-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="710fd-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-add-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="710fd-142">Java</span><span class="sxs-lookup"><span data-stu-id="710fd-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-add-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="710fd-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="710fd-143">Response</span></span>

<span data-ttu-id="710fd-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="710fd-144">The following is an example of the response.</span></span>

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


