---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: Publicar página
localization_priority: Normal
ms.openlocfilehash: 0b98f22dda2c4b08d04150b8b24126fdff5ca505
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836152"
---
# <a name="sitepage-publish"></a><span data-ttu-id="cf15e-102">sitePage: publicar</span><span class="sxs-lookup"><span data-stu-id="cf15e-102">sitePage: publish</span></span>

> <span data-ttu-id="cf15e-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cf15e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf15e-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cf15e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cf15e-105">Publique a versão mais recente de um recurso de [sitePage][] , o que disponibiliza a versão da página para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="cf15e-105">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="cf15e-106">Se a página está com check-out, check-in de página e publicá-lo.</span><span class="sxs-lookup"><span data-stu-id="cf15e-106">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="cf15e-107">Se a página é verificada com o chamador desta API, a página é automaticamente check-in e, em seguida, publicada.</span><span class="sxs-lookup"><span data-stu-id="cf15e-107">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="cf15e-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="cf15e-109">Permissions</span></span>

<span data-ttu-id="cf15e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf15e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf15e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf15e-112">Permission type</span></span>      | <span data-ttu-id="cf15e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf15e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf15e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf15e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cf15e-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf15e-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="cf15e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf15e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf15e-117">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf15e-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="cf15e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf15e-118">Application</span></span> | <span data-ttu-id="cf15e-119">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf15e-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf15e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf15e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="cf15e-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf15e-121">Request body</span></span>

<span data-ttu-id="cf15e-122">Esta mensagem não tem um corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf15e-122">This message does not have a request body.</span></span> <span data-ttu-id="cf15e-123">Qualquer corpo da solicitação enviado será ignorado.</span><span class="sxs-lookup"><span data-stu-id="cf15e-123">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="cf15e-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf15e-124">Response</span></span>

<span data-ttu-id="cf15e-125">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cf15e-125">If successful, the API call returns a `204 No Content`.</span></span>

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
