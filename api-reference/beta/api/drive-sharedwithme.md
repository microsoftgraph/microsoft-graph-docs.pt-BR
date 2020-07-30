---
author: JeremyKelley
description: Recupere uma coleção de recursos DriveItem que foram compartilhados com o proprietário de Drive.
ms.date: 09/10/2017
title: Listar arquivos compartilhados comigo
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e06497071d78d02df93338ed7cdbe67e6c67cbfe
ms.sourcegitcommit: ff3fd4ead2b864ce6abb79915a0488d0562347f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2020
ms.locfileid: "46524230"
---
# <a name="list-items-shared-with-the-signed-in-user"></a><span data-ttu-id="81217-103">Listar itens compartilhados com o usuário conectado</span><span class="sxs-lookup"><span data-stu-id="81217-103">List items shared with the signed-in user</span></span>

<span data-ttu-id="81217-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81217-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81217-105">Recupere uma coleção de recursos [DriveItem](../resources/driveitem.md) que foram compartilhados com o proprietário de [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="81217-105">Retrieve a collection of [DriveItem](../resources/driveitem.md) resources that have been shared with the owner of the [Drive](../resources/drive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="81217-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="81217-106">Permissions</span></span>

<span data-ttu-id="81217-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81217-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81217-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81217-109">Permission type</span></span>      | <span data-ttu-id="81217-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81217-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81217-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81217-111">Delegated (work or school account)</span></span> | <span data-ttu-id="81217-112">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81217-112">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="81217-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81217-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81217-114">Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81217-114">Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="81217-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81217-115">Application</span></span> | <span data-ttu-id="81217-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81217-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

<span data-ttu-id="81217-117">**Observação:** embora a solicitação /sharedWithMe tenha êxito com as permissões Files.Read ou Files.ReadWrite, algumas propriedades podem estar ausentes.</span><span class="sxs-lookup"><span data-stu-id="81217-117">**Note:** while the /sharedWithMe request will succeed with Files.Read or Files.ReadWrite permissions, some properties may be missing.</span></span>
<span data-ttu-id="81217-118">Além disso, sem uma das permissões **All**, os itens compartilhados retornados dessa API não ficarão acessíveis.</span><span class="sxs-lookup"><span data-stu-id="81217-118">Additionally, without one of the  **All** permissions, shared items returned from this API will not be accessible.</span></span>

## <a name="http-request"></a><span data-ttu-id="81217-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81217-119">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="81217-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="81217-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "shared-with-me", "scopes": "files.read", "target": "action" } -->

```msgraph-interactive
GET /me/drive/sharedWithMe
```
# <a name="c"></a>[<span data-ttu-id="81217-121">C#</span><span class="sxs-lookup"><span data-stu-id="81217-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shared-with-me-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81217-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81217-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shared-with-me-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81217-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81217-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shared-with-me-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="81217-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="81217-124">Response</span></span>

<span data-ttu-id="81217-p103">Isso retorna uma coleção de recursos [DriveItem](../resources/driveitem.md) que contêm DriveItem recursos compartilhados com o proprietário da unidade. Neste exemplo, como a unidade é a do usuário padrão, isso retorna itens compartilhados com o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="81217-p103">This returns a collection of [DriveItem](../resources/driveitem.md) resources which contain the DriveItem resources shared with the owner of the drive. In this example, since the drive is the user's default drive, this returns items shared with the signed in user.</span></span>

<!-- {"blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc",
      "remoteItem": {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    },
    {
      "id": "1312def",
      "remoteItem": {
        "id": "1991210caf!1991",
        "name": "Team Roster.xlsx",
        "file": { },
        "size": 37619,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="81217-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="81217-127">Remarks</span></span>

<span data-ttu-id="81217-p104">DriveItems retornados da ação **sharedWithMe** sempre incluirão a faceta [**remoteItem**](../resources/remoteitem.md), que indica que são itens de uma unidade diferente. Para acessar o recurso compartilhado DriveItem, você precisará fazer uma solicitação usando as informações fornecidas em **remoteItem** no seguinte formato:</span><span class="sxs-lookup"><span data-stu-id="81217-p104">DriveItems returned from the **sharedWithMe** action will always include the [**remoteItem**](../resources/remoteitem.md) facet which indicates they are items from a different drive. To access the shared DriveItem resource, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```
<span data-ttu-id="81217-130">Por padrão, **sharedWithMe** retorna itens compartilhados em seu próprio locatário.</span><span class="sxs-lookup"><span data-stu-id="81217-130">By default, **sharedWithMe** returns items shared within your own tenant.</span></span> <span data-ttu-id="81217-131">Para incluir itens compartilhados de locatários externos, acrescente `?allowexternal=true` à solicitação GET.</span><span class="sxs-lookup"><span data-stu-id="81217-131">To include items shared from external tenants, append `?allowexternal=true` to the GET request.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "List the items shared with the owner of a drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Sharing/Shared with me",
  "suppressions": [
  ]
}
-->
