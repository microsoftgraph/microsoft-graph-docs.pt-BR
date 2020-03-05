---
author: rahmit
description: Publicar a versão mais recente de um recurso sitePage, que torna a versão da página disponível para todos os usuários. Se a página estiver com check-out, faça check-in na página e publique-a. Se a página estiver com check-out para o chamador desta API, a página será automaticamente verificada e publicada.
ms.date: 09/10/2018
title: Publicar página
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 90d08b3f8fae2ed186d1809b4318eec7ef9cf5dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453164"
---
# <a name="sitepage-publish"></a><span data-ttu-id="d9a4a-105">sitePage: publish</span><span class="sxs-lookup"><span data-stu-id="d9a4a-105">sitePage: publish</span></span>

<span data-ttu-id="d9a4a-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d9a4a-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9a4a-107">Publicar a versão mais recente de um recurso [sitePage][] , que torna a versão da página disponível para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="d9a4a-107">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="d9a4a-108">Se a página estiver com check-out, faça check-in na página e publique-a.</span><span class="sxs-lookup"><span data-stu-id="d9a4a-108">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="d9a4a-109">Se a página estiver com check-out para o chamador desta API, a página será automaticamente verificada e publicada.</span><span class="sxs-lookup"><span data-stu-id="d9a4a-109">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="d9a4a-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9a4a-111">Permissions</span></span>

<span data-ttu-id="d9a4a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9a4a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9a4a-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9a4a-114">Permission type</span></span>      | <span data-ttu-id="d9a4a-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9a4a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9a4a-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9a4a-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d9a4a-117">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9a4a-117">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d9a4a-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9a4a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9a4a-119">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9a4a-119">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d9a4a-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9a4a-120">Application</span></span> | <span data-ttu-id="d9a4a-121">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9a4a-121">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9a4a-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9a4a-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="d9a4a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9a4a-123">Request body</span></span>

<span data-ttu-id="d9a4a-124">Esta mensagem não tem um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9a4a-124">This message does not have a request body.</span></span> <span data-ttu-id="d9a4a-125">Qualquer corpo de solicitação enviado será ignorado.</span><span class="sxs-lookup"><span data-stu-id="d9a4a-125">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="d9a4a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9a4a-126">Response</span></span>

<span data-ttu-id="d9a4a-127">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d9a4a-127">If successful, the API call returns a `204 No Content`.</span></span>

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
