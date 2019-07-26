---
title: Adicionar aplicativo à equipe
description: Instalar um aplicativo para a equipe especificada.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 07e8a5989050a0323fdbcde8027e6c89bef0d454
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908458"
---
# <a name="add-app-to-team"></a><span data-ttu-id="02d28-103">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="02d28-103">Add app to team</span></span>

<span data-ttu-id="02d28-104">Instalar um [aplicativo](../resources/teamsapp.md) para a [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="02d28-104">Install an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="02d28-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="02d28-105">Permissions</span></span>

<span data-ttu-id="02d28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02d28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02d28-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02d28-108">Permission type</span></span>      | <span data-ttu-id="02d28-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02d28-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02d28-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02d28-110">Delegated (work or school account)</span></span> | <span data-ttu-id="02d28-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02d28-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="02d28-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02d28-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02d28-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02d28-113">Not supported.</span></span>    |
|<span data-ttu-id="02d28-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02d28-114">Application</span></span> | <span data-ttu-id="02d28-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02d28-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02d28-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02d28-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="02d28-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02d28-117">Request headers</span></span>

| <span data-ttu-id="02d28-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02d28-118">Header</span></span>       | <span data-ttu-id="02d28-119">Valor</span><span class="sxs-lookup"><span data-stu-id="02d28-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="02d28-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="02d28-120">Authorization</span></span>  | <span data-ttu-id="02d28-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02d28-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="02d28-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02d28-123">Request body</span></span>

| <span data-ttu-id="02d28-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02d28-124">Property</span></span>   | <span data-ttu-id="02d28-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="02d28-125">Type</span></span> |<span data-ttu-id="02d28-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="02d28-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02d28-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="02d28-127">teamsApp</span></span>| [<span data-ttu-id="02d28-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="02d28-128">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="02d28-129">O aplicativo a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="02d28-129">The app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="02d28-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="02d28-130">Response</span></span>

<span data-ttu-id="02d28-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02d28-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02d28-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02d28-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="02d28-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02d28-134">Request</span></span>

<span data-ttu-id="02d28-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="02d28-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```

### <a name="response"></a><span data-ttu-id="02d28-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="02d28-136">Response</span></span>

<span data-ttu-id="02d28-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="02d28-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
