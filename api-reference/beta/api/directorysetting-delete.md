---
title: Excluir uma configuração de diretório
description: Excluir uma configuração de diretório.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ea7939423dd883f77619eb88a95a728afd58944e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325880"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="b9a6c-103">Excluir uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="b9a6c-103">Delete a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9a6c-104">Excluir uma configuração de diretório.</span><span class="sxs-lookup"><span data-stu-id="b9a6c-104">Delete a directory setting.</span></span>

> <span data-ttu-id="b9a6c-105">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="b9a6c-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="b9a6c-106">A versão/v1.0 dessa API foi renomeada para *excluir groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="b9a6c-106">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9a6c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b9a6c-107">Permissions</span></span>
<span data-ttu-id="b9a6c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9a6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9a6c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9a6c-110">Permission type</span></span>      | <span data-ttu-id="b9a6c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9a6c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9a6c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9a6c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b9a6c-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b9a6c-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b9a6c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9a6c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9a6c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9a6c-115">Not supported.</span></span>    |
|<span data-ttu-id="b9a6c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9a6c-116">Application</span></span> | <span data-ttu-id="b9a6c-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9a6c-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9a6c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9a6c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="b9a6c-119">Excluir uma configuração específica de todo o locatário ou grupo</span><span class="sxs-lookup"><span data-stu-id="b9a6c-119">Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="b9a6c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a6c-120">Request headers</span></span>
| <span data-ttu-id="b9a6c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b9a6c-121">Name</span></span>       | <span data-ttu-id="b9a6c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9a6c-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b9a6c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9a6c-123">Authorization</span></span>  | <span data-ttu-id="b9a6c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9a6c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9a6c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a6c-126">Request body</span></span>
<span data-ttu-id="b9a6c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9a6c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9a6c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9a6c-128">Response</span></span>

<span data-ttu-id="b9a6c-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9a6c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9a6c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9a6c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9a6c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a6c-132">Request</span></span>
<span data-ttu-id="b9a6c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9a6c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="b9a6c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9a6c-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
