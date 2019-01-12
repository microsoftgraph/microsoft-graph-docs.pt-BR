---
title: Excluir calendarGroup
description: Exclui um grupo de calendários diferente do grupo de calendários padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 7200021a105e600f2e1e28444ae2ae4c79df47b3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922526"
---
# <a name="delete-calendargroup"></a><span data-ttu-id="968d9-103">Excluir calendarGroup</span><span class="sxs-lookup"><span data-stu-id="968d9-103">Delete calendarGroup</span></span>

> <span data-ttu-id="968d9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="968d9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="968d9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="968d9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="968d9-106">Exclui um grupo de calendários diferente do grupo de calendários padrão.</span><span class="sxs-lookup"><span data-stu-id="968d9-106">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="968d9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="968d9-107">Permissions</span></span>

<span data-ttu-id="968d9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="968d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="968d9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="968d9-110">Permission type</span></span>                        | <span data-ttu-id="968d9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="968d9-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="968d9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="968d9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="968d9-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="968d9-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="968d9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="968d9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="968d9-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="968d9-115">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="968d9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="968d9-116">Application</span></span>                            | <span data-ttu-id="968d9-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="968d9-117">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="968d9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="968d9-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="968d9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="968d9-119">Request headers</span></span>

| <span data-ttu-id="968d9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="968d9-120">Name</span></span>          | <span data-ttu-id="968d9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="968d9-121">Type</span></span>   | <span data-ttu-id="968d9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="968d9-122">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="968d9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="968d9-123">Authorization</span></span> | <span data-ttu-id="968d9-124">string</span><span class="sxs-lookup"><span data-stu-id="968d9-124">string</span></span> | <span data-ttu-id="968d9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="968d9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="968d9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="968d9-127">Request body</span></span>

<span data-ttu-id="968d9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="968d9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="968d9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="968d9-129">Response</span></span>

<span data-ttu-id="968d9-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="968d9-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="968d9-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="968d9-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="968d9-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="968d9-133">Request</span></span>

<span data-ttu-id="968d9-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="968d9-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="968d9-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="968d9-135">Response</span></span>

<span data-ttu-id="968d9-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="968d9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
