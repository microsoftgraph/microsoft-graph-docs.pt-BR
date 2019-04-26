---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: Publicar página
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d9bf699c0038e785a11560ee7326cfb2324345f3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335882"
---
# <a name="sitepage-publish"></a><span data-ttu-id="ce106-102">sitePage: publish</span><span class="sxs-lookup"><span data-stu-id="ce106-102">sitePage: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce106-103">Publicar a versão mais recente de um recurso [sitePage][] , que torna a versão da página disponível para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="ce106-103">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="ce106-104">Se a página estiver com check-out, faça check-in na página e publique-a.</span><span class="sxs-lookup"><span data-stu-id="ce106-104">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="ce106-105">Se a página estiver com check-out para o chamador desta API, a página será automaticamente verificada e publicada.</span><span class="sxs-lookup"><span data-stu-id="ce106-105">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="ce106-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce106-107">Permissions</span></span>

<span data-ttu-id="ce106-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce106-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce106-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce106-110">Permission type</span></span>      | <span data-ttu-id="ce106-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce106-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce106-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce106-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ce106-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce106-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ce106-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce106-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce106-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce106-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ce106-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce106-116">Application</span></span> | <span data-ttu-id="ce106-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce106-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce106-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce106-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="ce106-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce106-119">Request body</span></span>

<span data-ttu-id="ce106-120">Esta mensagem não tem um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce106-120">This message does not have a request body.</span></span> <span data-ttu-id="ce106-121">Qualquer corpo de solicitação enviado será ignorado.</span><span class="sxs-lookup"><span data-stu-id="ce106-121">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="ce106-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce106-122">Response</span></span>

<span data-ttu-id="ce106-123">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ce106-123">If successful, the API call returns a `204 No Content`.</span></span>

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
