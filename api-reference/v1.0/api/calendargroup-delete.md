---
title: Excluir calendarGroup
description: Exclui um grupo de calendários diferente do grupo de calendários padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f1dded8885f99646d48ddf309ff12e64d61988e1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978932"
---
# <a name="delete-calendargroup"></a><span data-ttu-id="2970d-103">Excluir calendarGroup</span><span class="sxs-lookup"><span data-stu-id="2970d-103">Delete calendarGroup</span></span>

<span data-ttu-id="2970d-104">Exclui um grupo de calendários diferente do grupo de calendários padrão.</span><span class="sxs-lookup"><span data-stu-id="2970d-104">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="2970d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2970d-105">Permissions</span></span>

<span data-ttu-id="2970d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2970d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2970d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2970d-108">Permission type</span></span>                        | <span data-ttu-id="2970d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2970d-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="2970d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2970d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2970d-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2970d-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="2970d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2970d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2970d-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2970d-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="2970d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2970d-114">Application</span></span>                            | <span data-ttu-id="2970d-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2970d-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2970d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2970d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2970d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2970d-117">Request headers</span></span>

| <span data-ttu-id="2970d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2970d-118">Name</span></span>          | <span data-ttu-id="2970d-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="2970d-119">Type</span></span>   | <span data-ttu-id="2970d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2970d-120">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="2970d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2970d-121">Authorization</span></span> | <span data-ttu-id="2970d-122">string</span><span class="sxs-lookup"><span data-stu-id="2970d-122">string</span></span> | <span data-ttu-id="2970d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2970d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2970d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2970d-125">Request body</span></span>

<span data-ttu-id="2970d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2970d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2970d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="2970d-127">Response</span></span>

<span data-ttu-id="2970d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2970d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2970d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2970d-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2970d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2970d-131">Request</span></span>

<span data-ttu-id="2970d-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2970d-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="2970d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2970d-133">Response</span></span>

<span data-ttu-id="2970d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2970d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Delete calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
