---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: Publicar página
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a00a69542c2b59b1b268433b08656c87d194feb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545213"
---
# <a name="sitepage-publish"></a><span data-ttu-id="98f11-102">sitePage: publish</span><span class="sxs-lookup"><span data-stu-id="98f11-102">sitePage: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98f11-103">Publicar a versão mais recente de um recurso [sitePage][] , que torna a versão da página disponível para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="98f11-103">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="98f11-104">Se a página estiver com check-out, faça check-in na página e publique-a.</span><span class="sxs-lookup"><span data-stu-id="98f11-104">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="98f11-105">Se a página estiver com check-out para o chamador desta API, a página será automaticamente verificada e publicada.</span><span class="sxs-lookup"><span data-stu-id="98f11-105">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="98f11-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="98f11-107">Permissions</span></span>

<span data-ttu-id="98f11-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98f11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98f11-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98f11-110">Permission type</span></span>      | <span data-ttu-id="98f11-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="98f11-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98f11-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98f11-112">Delegated (work or school account)</span></span> | <span data-ttu-id="98f11-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98f11-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="98f11-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98f11-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98f11-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98f11-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="98f11-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98f11-116">Application</span></span> | <span data-ttu-id="98f11-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98f11-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98f11-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98f11-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="98f11-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98f11-119">Request body</span></span>

<span data-ttu-id="98f11-120">Esta mensagem não tem um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="98f11-120">This message does not have a request body.</span></span> <span data-ttu-id="98f11-121">Qualquer corpo de solicitação enviado será ignorado.</span><span class="sxs-lookup"><span data-stu-id="98f11-121">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="98f11-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="98f11-122">Response</span></span>

<span data-ttu-id="98f11-123">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="98f11-123">If successful, the API call returns a `204 No Content`.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/sitepage-publish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
