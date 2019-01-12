---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: Publicar página
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 8e59a7aea74e165945757f2513102a66baf64be1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920237"
---
# <a name="sitepage-publish"></a><span data-ttu-id="0361d-102">sitePage: publicar</span><span class="sxs-lookup"><span data-stu-id="0361d-102">sitePage: publish</span></span>

> <span data-ttu-id="0361d-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0361d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0361d-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0361d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0361d-105">Publique a versão mais recente de um recurso de [sitePage][] , o que disponibiliza a versão da página para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="0361d-105">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="0361d-106">Se a página está com check-out, check-in de página e publicá-lo.</span><span class="sxs-lookup"><span data-stu-id="0361d-106">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="0361d-107">Se a página é verificada com o chamador desta API, a página é automaticamente check-in e, em seguida, publicada.</span><span class="sxs-lookup"><span data-stu-id="0361d-107">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="0361d-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="0361d-109">Permissions</span></span>

<span data-ttu-id="0361d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0361d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0361d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0361d-112">Permission type</span></span>      | <span data-ttu-id="0361d-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0361d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0361d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0361d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0361d-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0361d-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0361d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0361d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0361d-117">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0361d-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="0361d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0361d-118">Application</span></span> | <span data-ttu-id="0361d-119">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0361d-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0361d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0361d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="0361d-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0361d-121">Request body</span></span>

<span data-ttu-id="0361d-122">Esta mensagem não tem um corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0361d-122">This message does not have a request body.</span></span> <span data-ttu-id="0361d-123">Qualquer corpo da solicitação enviado será ignorado.</span><span class="sxs-lookup"><span data-stu-id="0361d-123">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="0361d-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="0361d-124">Response</span></span>

<span data-ttu-id="0361d-125">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0361d-125">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Publish a page.",
  "keywords": "publish page",
  "section": "documentation",
  "tocPath": "Pages/Publish"
} -->
