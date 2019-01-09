---
title: Excluir outlookTask
description: Exclua a tarefa especificada do Outlook na caixa de correio do usuário.
ms.openlocfilehash: cab78b8fea63c5044cc6faa6a1e4f09dd960bfd6
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771776"
---
# <a name="delete-outlooktask"></a><span data-ttu-id="5395f-103">Excluir outlookTask</span><span class="sxs-lookup"><span data-stu-id="5395f-103">Delete outlookTask</span></span>

> <span data-ttu-id="5395f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5395f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5395f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5395f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5395f-106">Exclua a tarefa especificada do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="5395f-106">Delete the specified Outlook task in the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="5395f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5395f-107">Permissions</span></span>

<span data-ttu-id="5395f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5395f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5395f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5395f-110">Permission type</span></span>      | <span data-ttu-id="5395f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5395f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5395f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5395f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5395f-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5395f-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="5395f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5395f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5395f-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5395f-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="5395f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5395f-116">Application</span></span> | <span data-ttu-id="5395f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5395f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5395f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5395f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/{id}
DELETE /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5395f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5395f-119">Request headers</span></span>

| <span data-ttu-id="5395f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5395f-120">Name</span></span>       | <span data-ttu-id="5395f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5395f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5395f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5395f-122">Authorization</span></span>  | <span data-ttu-id="5395f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5395f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5395f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5395f-125">Request body</span></span>

<span data-ttu-id="5395f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5395f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5395f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5395f-127">Response</span></span>

<span data-ttu-id="5395f-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5395f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5395f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5395f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5395f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5395f-131">Request</span></span>

<span data-ttu-id="5395f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5395f-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktask"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADIyAAAhrb_QAAA=')
```

### <a name="response"></a><span data-ttu-id="5395f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5395f-133">Response</span></span>

<span data-ttu-id="5395f-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5395f-134">Here is an example of the response.</span></span>
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
  "description": "Delete outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->