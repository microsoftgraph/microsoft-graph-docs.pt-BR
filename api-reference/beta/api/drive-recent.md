---
author: JeremyKelley
description: Liste um conjunto de itens que foram usados recentemente pelo usuário conectado.
ms.date: 09/10/2017
title: Listar arquivos recentes
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 745e002342eca8c04a990d49e7a2cb0daa1c42dc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957294"
---
# <a name="list-recent-files"></a><span data-ttu-id="ae16f-103">Liste arquivos recentes</span><span class="sxs-lookup"><span data-stu-id="ae16f-103">List recent files</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae16f-p101">Listar uma coleção de itens que foram usados recentemente pelo usuário conectado. Esta coleção inclui itens que estão na unidade do usuário, assim como itens aos quais ele tem acesso por meio de outras unidades.</span><span class="sxs-lookup"><span data-stu-id="ae16f-p101">List a set of items that have been recently used by the signed in user. This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae16f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ae16f-106">Permissions</span></span>

<span data-ttu-id="ae16f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae16f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae16f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae16f-109">Permission type</span></span>      | <span data-ttu-id="ae16f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae16f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae16f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae16f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ae16f-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae16f-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ae16f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae16f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae16f-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae16f-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ae16f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae16f-115">Application</span></span> | <span data-ttu-id="ae16f-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae16f-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae16f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae16f-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ae16f-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae16f-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request",
       "name": "view-recent-files", 
       "scopes": "files.read",
       "target": "action" } -->

```http
GET /me/drive/recent
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ae16f-119">C#</span><span class="sxs-lookup"><span data-stu-id="ae16f-119">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/view-recent-files-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ae16f-120">Javascript</span><span class="sxs-lookup"><span data-stu-id="ae16f-120">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/view-recent-files-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ae16f-121">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ae16f-121">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/view-recent-files-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ae16f-122">Java</span><span class="sxs-lookup"><span data-stu-id="ae16f-122">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/view-recent-files-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="ae16f-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae16f-123">Response</span></span>

<span data-ttu-id="ae16f-124">Esse método retorna uma coleção de recursos [DriveItem](../resources/driveitem.md) para itens que o proprietário da unidade acessou recentemente.</span><span class="sxs-lookup"><span data-stu-id="ae16f-124">This method returns a collection of [DriveItem](../resources/driveitem.md) resources for items which the owner of the drive has recently accessed.</span></span>

<!-- { "blockType": "response",
       "@odata.type": "Collection(microsoft.graph.driveItem)",
       "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "remoteItem":
      {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      },
      "fileSystemInfo": {
        "lastAccessedDateTime": "2017-02-20T19:13:00Z"
      }
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "file": { },
      "size": 37810,
      "parentReference": {
        "driveId": "1312def",
        "id": "1312def!123"
      },
      "fileSystemInfo": {
        "lastAccessedDateTime": "2017-02-20T16:43:21Z"
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="ae16f-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="ae16f-125">Remarks</span></span>

<span data-ttu-id="ae16f-p103">Alguns driveItems retornados da ação **recent** incluirão a faceta **remoteItem** que indica que eles são itens de outra unidade. Para acessar o objeto driveItem original, você precisará fazer uma solicitação usando as informações fornecidas em **remoteItem** no seguinte formato:</span><span class="sxs-lookup"><span data-stu-id="ae16f-p103">Some driveItems returned from the **recent** action will include the **remoteItem** facet which indicates they are items from another drive. To access the original driveItem object, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!--
{
  "type": "#page.annotation",
  "description": "Retrieve a list of recently used files for the owner of the drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Drives/Recent files",
  "suppressions": [
  ]
}
-->
