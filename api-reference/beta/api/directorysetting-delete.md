---
title: Excluir uma configuração de diretório
description: Exclua uma configuração de diretório.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bebe1604de27b7bfebededd5a470d402f0a36e55
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975439"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="72032-103">Excluir uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="72032-103">Delete a directory setting</span></span>

> <span data-ttu-id="72032-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="72032-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72032-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="72032-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="72032-106">Exclua uma configuração de diretório.</span><span class="sxs-lookup"><span data-stu-id="72032-106">Delete a directory setting.</span></span>

> <span data-ttu-id="72032-107">**Observação**: A versão de /beta desse API é só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="72032-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="72032-108">A versão de /v1.0 desse API foi renomeada para *Excluir groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="72032-108">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="72032-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="72032-109">Permissions</span></span>
<span data-ttu-id="72032-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72032-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72032-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72032-112">Permission type</span></span>      | <span data-ttu-id="72032-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72032-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72032-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72032-114">Delegated (work or school account)</span></span> | <span data-ttu-id="72032-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="72032-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="72032-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72032-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72032-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72032-117">Not supported.</span></span>    |
|<span data-ttu-id="72032-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72032-118">Application</span></span> | <span data-ttu-id="72032-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72032-119">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="72032-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72032-120">HTTP request</span></span>
<span data-ttu-id="72032-121"><!-- { "blockType": "ignored" } -->Excluir um locatário todo específico ou configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="72032-121"><!-- { "blockType": "ignored" } --> Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="72032-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72032-122">Request headers</span></span>
| <span data-ttu-id="72032-123">Nome</span><span class="sxs-lookup"><span data-stu-id="72032-123">Name</span></span>       | <span data-ttu-id="72032-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="72032-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="72032-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="72032-125">Authorization</span></span>  | <span data-ttu-id="72032-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72032-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72032-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72032-128">Request body</span></span>
<span data-ttu-id="72032-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72032-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72032-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="72032-130">Response</span></span>

<span data-ttu-id="72032-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72032-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72032-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72032-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72032-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72032-134">Request</span></span>
<span data-ttu-id="72032-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72032-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="72032-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="72032-136">Response</span></span>
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
  "description": "Delete directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
