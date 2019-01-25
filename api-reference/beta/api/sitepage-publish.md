---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: Publicar página
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a00a69542c2b59b1b268433b08656c87d194feb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507527"
---
# <a name="sitepage-publish"></a><span data-ttu-id="53c68-102">sitePage: publicar</span><span class="sxs-lookup"><span data-stu-id="53c68-102">sitePage: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53c68-103">Publique a versão mais recente de um recurso de [sitePage][] , o que disponibiliza a versão da página para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="53c68-103">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="53c68-104">Se a página está com check-out, check-in de página e publicá-lo.</span><span class="sxs-lookup"><span data-stu-id="53c68-104">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="53c68-105">Se a página é verificada com o chamador desta API, a página é automaticamente check-in e, em seguida, publicada.</span><span class="sxs-lookup"><span data-stu-id="53c68-105">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="53c68-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="53c68-107">Permissions</span></span>

<span data-ttu-id="53c68-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53c68-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53c68-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53c68-110">Permission type</span></span>      | <span data-ttu-id="53c68-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="53c68-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53c68-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53c68-112">Delegated (work or school account)</span></span> | <span data-ttu-id="53c68-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53c68-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="53c68-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53c68-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53c68-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53c68-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="53c68-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53c68-116">Application</span></span> | <span data-ttu-id="53c68-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53c68-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53c68-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53c68-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="53c68-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53c68-119">Request body</span></span>

<span data-ttu-id="53c68-120">Esta mensagem não tem um corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53c68-120">This message does not have a request body.</span></span> <span data-ttu-id="53c68-121">Qualquer corpo da solicitação enviado será ignorado.</span><span class="sxs-lookup"><span data-stu-id="53c68-121">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="53c68-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="53c68-122">Response</span></span>

<span data-ttu-id="53c68-123">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="53c68-123">If successful, the API call returns a `204 No Content`.</span></span>

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
