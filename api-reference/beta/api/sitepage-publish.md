---
author: rahmit
description: Publicar a versão mais recente de um recurso sitePage, que torna a versão da página disponível para todos os usuários. Se a página estiver com check-out, faça check-in na página e publique-a. Se a página estiver com check-out para o chamador desta API, a página será automaticamente verificada e publicada.
ms.date: 09/10/2018
title: Publicar página
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5f4404b33a54979271750d4074a9c6da235966ea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991209"
---
# <a name="sitepage-publish"></a><span data-ttu-id="0f19b-105">sitePage: publish</span><span class="sxs-lookup"><span data-stu-id="0f19b-105">sitePage: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f19b-106">Publicar a versão mais recente de um recurso [sitePage][] , que torna a versão da página disponível para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="0f19b-106">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="0f19b-107">Se a página estiver com check-out, faça check-in na página e publique-a.</span><span class="sxs-lookup"><span data-stu-id="0f19b-107">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="0f19b-108">Se a página estiver com check-out para o chamador desta API, a página será automaticamente verificada e publicada.</span><span class="sxs-lookup"><span data-stu-id="0f19b-108">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="0f19b-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f19b-110">Permissions</span></span>

<span data-ttu-id="0f19b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f19b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f19b-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f19b-113">Permission type</span></span>      | <span data-ttu-id="0f19b-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f19b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f19b-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f19b-115">Delegated (work or school account)</span></span> | <span data-ttu-id="0f19b-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f19b-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0f19b-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f19b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f19b-118">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f19b-118">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="0f19b-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f19b-119">Application</span></span> | <span data-ttu-id="0f19b-120">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f19b-120">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f19b-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f19b-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="0f19b-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f19b-122">Request body</span></span>

<span data-ttu-id="0f19b-123">Esta mensagem não tem um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f19b-123">This message does not have a request body.</span></span> <span data-ttu-id="0f19b-124">Qualquer corpo de solicitação enviado será ignorado.</span><span class="sxs-lookup"><span data-stu-id="0f19b-124">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="0f19b-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f19b-125">Response</span></span>

<span data-ttu-id="0f19b-126">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0f19b-126">If successful, the API call returns a `204 No Content`.</span></span>

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
