---
title: Instalar o aplicativo para o usuário
description: Instalar um aplicativo no escopo pessoal do usuário especificado.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 009d2efe115d8b07f9bdead07965d402db65e65a
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908541"
---
# <a name="install-app-for-user"></a><span data-ttu-id="e3c0c-103">Instalar o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="e3c0c-103">Install app for user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3c0c-104">Instalar um [aplicativo](../resources/teamsapp.md) no escopo pessoal do [usuário](../resources/user.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="e3c0c-104">Install an [app](../resources/teamsapp.md) in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3c0c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e3c0c-105">Permissions</span></span>

<span data-ttu-id="e3c0c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3c0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3c0c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3c0c-108">Permission type</span></span>      | <span data-ttu-id="e3c0c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3c0c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3c0c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3c0c-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e3c0c-111">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3c0c-111">User.ReadWrite.All, Directory.ReadWrite.All</span></span>     |
|<span data-ttu-id="e3c0c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3c0c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3c0c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3c0c-113">Not supported.</span></span>    |
|<span data-ttu-id="e3c0c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3c0c-114">Application</span></span> | <span data-ttu-id="e3c0c-115">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3c0c-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3c0c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3c0c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="e3c0c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3c0c-117">Request headers</span></span>

| <span data-ttu-id="e3c0c-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e3c0c-118">Header</span></span>       | <span data-ttu-id="e3c0c-119">Valor</span><span class="sxs-lookup"><span data-stu-id="e3c0c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e3c0c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3c0c-120">Authorization</span></span>  | <span data-ttu-id="e3c0c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3c0c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e3c0c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3c0c-123">Request body</span></span>

<span data-ttu-id="e3c0c-124">O corpo da solicitação deve conter a ID do aplicativo de catálogo existente a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="e3c0c-124">The request body should contain the ID of the existing catalog app to be added.</span></span>

| <span data-ttu-id="e3c0c-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3c0c-125">Property</span></span>   | <span data-ttu-id="e3c0c-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3c0c-126">Type</span></span> |<span data-ttu-id="e3c0c-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3c0c-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3c0c-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e3c0c-128">teamsApp</span></span>|<span data-ttu-id="e3c0c-129">String</span><span class="sxs-lookup"><span data-stu-id="e3c0c-129">String</span></span>|<span data-ttu-id="e3c0c-130">A ID do aplicativo a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="e3c0c-130">The ID of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="e3c0c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3c0c-131">Response</span></span>

<span data-ttu-id="e3c0c-p103">Se bem-sucedido, este método retorna um código de resposta `201 Created`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3c0c-p103">If successful, this method returns a `201 Created` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3c0c-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3c0c-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3c0c-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3c0c-135">Request</span></span>

<span data-ttu-id="e3c0c-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3c0c-136">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e3c0c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3c0c-137">Response</span></span>

<span data-ttu-id="e3c0c-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e3c0c-138">The following is an example of the response.</span></span>

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
