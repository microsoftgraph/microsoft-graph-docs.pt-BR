---
author: rahmit
description: Publicar a versão mais recente de um recurso sitePage, que torna a versão da página disponível para todos os usuários. Se a página estiver com check-out, faça check-in na página e publique-a. Se a página estiver com check-out para o chamador desta API, a página será automaticamente verificada e publicada.
ms.date: 09/10/2018
title: Publicar página
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e40f864ce224916a2c60e5c82e0aecbfff213fbc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044375"
---
# <a name="sitepage-publish"></a><span data-ttu-id="488ee-105">sitePage: publish</span><span class="sxs-lookup"><span data-stu-id="488ee-105">sitePage: publish</span></span>

<span data-ttu-id="488ee-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="488ee-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="488ee-107">Publicar a versão mais recente de um recurso [sitePage][] , que torna a versão da página disponível para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="488ee-107">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="488ee-108">Se a página estiver com check-out, faça check-in na página e publique-a.</span><span class="sxs-lookup"><span data-stu-id="488ee-108">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="488ee-109">Se a página estiver com check-out para o chamador desta API, a página será automaticamente verificada e publicada.</span><span class="sxs-lookup"><span data-stu-id="488ee-109">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="488ee-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="488ee-111">Permissions</span></span>

<span data-ttu-id="488ee-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="488ee-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="488ee-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="488ee-114">Permission type</span></span>      | <span data-ttu-id="488ee-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="488ee-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="488ee-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="488ee-116">Delegated (work or school account)</span></span> | <span data-ttu-id="488ee-117">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="488ee-117">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="488ee-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="488ee-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="488ee-119">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="488ee-119">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="488ee-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="488ee-120">Application</span></span> | <span data-ttu-id="488ee-121">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="488ee-121">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="488ee-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="488ee-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="488ee-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="488ee-123">Request body</span></span>

<span data-ttu-id="488ee-124">Esta mensagem não tem um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="488ee-124">This message does not have a request body.</span></span> <span data-ttu-id="488ee-125">Qualquer corpo de solicitação enviado será ignorado.</span><span class="sxs-lookup"><span data-stu-id="488ee-125">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="488ee-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="488ee-126">Response</span></span>

<span data-ttu-id="488ee-127">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="488ee-127">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


<!--
{
  "type": "#page.annotation",
  "description": "Publish a page.",
  "keywords": "publish page",
  "section": "documentation",
  "tocPath": "Pages/Publish",
  "suppressions": []
}
-->


