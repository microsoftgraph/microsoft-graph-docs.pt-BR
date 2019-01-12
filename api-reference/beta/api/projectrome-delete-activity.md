---
title: Excluir uma atividade
description: Exclua uma atividade do usuário existente para seu aplicativo.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 8b4bf0b09cb5796e1db8e22ced7e471bdd5117f4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925746"
---
# <a name="delete-an-activity"></a><span data-ttu-id="89c73-103">Excluir uma atividade</span><span class="sxs-lookup"><span data-stu-id="89c73-103">Delete an activity</span></span>

> <span data-ttu-id="89c73-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="89c73-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89c73-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="89c73-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="89c73-106">Exclua uma atividade do usuário existente para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="89c73-106">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="89c73-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="89c73-107">Permissions</span></span>

<span data-ttu-id="89c73-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89c73-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="89c73-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89c73-110">Permission type</span></span>      | <span data-ttu-id="89c73-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="89c73-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89c73-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89c73-112">Delegated (work or school account)</span></span> | <span data-ttu-id="89c73-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="89c73-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="89c73-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89c73-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89c73-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="89c73-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="89c73-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89c73-116">Application</span></span> | <span data-ttu-id="89c73-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89c73-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89c73-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89c73-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="89c73-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89c73-119">Request headers</span></span>

|<span data-ttu-id="89c73-120">Nome</span><span class="sxs-lookup"><span data-stu-id="89c73-120">Name</span></span> | <span data-ttu-id="89c73-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="89c73-121">Type</span></span> | <span data-ttu-id="89c73-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="89c73-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="89c73-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="89c73-123">Authorization</span></span> | <span data-ttu-id="89c73-124">string</span><span class="sxs-lookup"><span data-stu-id="89c73-124">string</span></span> | <span data-ttu-id="89c73-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89c73-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="89c73-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89c73-127">Request body</span></span>

<span data-ttu-id="89c73-128">Nenhum corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89c73-128">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="89c73-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="89c73-129">Response</span></span>

<span data-ttu-id="89c73-130">Se tiver êxito, este método retornará o `204 No Content` código de resposta se a atividade foi excluída.</span><span class="sxs-lookup"><span data-stu-id="89c73-130">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="89c73-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89c73-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="89c73-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89c73-132">Request</span></span>

<span data-ttu-id="89c73-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89c73-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/activities/13881113971988980728/
```

##### <a name="response"></a><span data-ttu-id="89c73-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="89c73-134">Response</span></span>

<span data-ttu-id="89c73-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89c73-135">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
