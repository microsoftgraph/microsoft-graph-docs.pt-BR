---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Listar arquivos compartilhados comigo
localization_priority: Priority
ms.prod: sharepoint
description: Recupere uma coleção de recursos DriveItem que foram compartilhados com o proprietário de Drive.
doc_type: apiPageType
ms.openlocfilehash: ded63a41a5d6d59e547ea914988238846e21c214
ms.sourcegitcommit: ff3fd4ead2b864ce6abb79915a0488d0562347f8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2020
ms.locfileid: "46524321"
---
# <a name="list-items-shared-with-the-signed-in-user"></a><span data-ttu-id="af88c-103">Listar itens compartilhados com o usuário conectado</span><span class="sxs-lookup"><span data-stu-id="af88c-103">List items shared with the signed-in user</span></span>

<span data-ttu-id="af88c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af88c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="af88c-105">Recupere uma coleção de recursos [DriveItem](../resources/driveitem.md) que foram compartilhados com o proprietário de [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="af88c-105">Retrieve a collection of [DriveItem](../resources/driveitem.md) resources that have been shared with the owner of the [Drive](../resources/drive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="af88c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="af88c-106">Permissions</span></span>

<span data-ttu-id="af88c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af88c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af88c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af88c-109">Permission type</span></span>      | <span data-ttu-id="af88c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af88c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af88c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af88c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="af88c-112">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af88c-112">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="af88c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af88c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af88c-114">Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af88c-114">Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="af88c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af88c-115">Application</span></span> | <span data-ttu-id="af88c-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af88c-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

<span data-ttu-id="af88c-117">**Observação:** embora a solicitação /sharedWithMe tenha êxito com as permissões Files.Read ou Files.ReadWrite, algumas propriedades podem estar ausentes.</span><span class="sxs-lookup"><span data-stu-id="af88c-117">**Note:** while the /sharedWithMe request will succeed with Files.Read or Files.ReadWrite permissions, some properties may be missing.</span></span>
<span data-ttu-id="af88c-118">Além disso, sem uma das permissões **All**, os itens compartilhados retornados dessa API não ficarão acessíveis.</span><span class="sxs-lookup"><span data-stu-id="af88c-118">Additionally, without one of the  **All** permissions, shared items returned from this API will not be accessible.</span></span>

## <a name="http-request"></a><span data-ttu-id="af88c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af88c-119">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="af88c-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="af88c-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "shared-with-me", "scopes": "files.read", "tags": "service.graph", "target": "action" } -->

```msgraph-interactive
GET /me/drive/sharedWithMe
```
# <a name="c"></a>[<span data-ttu-id="af88c-121">C#</span><span class="sxs-lookup"><span data-stu-id="af88c-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shared-with-me-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af88c-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af88c-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shared-with-me-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af88c-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af88c-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shared-with-me-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="af88c-124">Java</span><span class="sxs-lookup"><span data-stu-id="af88c-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shared-with-me-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="af88c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="af88c-125">Response</span></span>

<span data-ttu-id="af88c-p103">Isso retorna uma coleção de recursos [DriveItem](../resources/driveitem.md) que contêm DriveItem recursos compartilhados com o proprietário da unidade. Neste exemplo, como a unidade é a do usuário padrão, isso retorna itens compartilhados com o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="af88c-p103">This returns a collection of [DriveItem](../resources/driveitem.md) resources which contain the DriveItem resources shared with the owner of the drive. In this example, since the drive is the user's default drive, this returns items shared with the signed in user.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="af88c-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="af88c-128">Remarks</span></span>

<span data-ttu-id="af88c-p104">DriveItems retornados da ação **sharedWithMe** sempre incluirão a faceta [**remoteItem**](../resources/remoteitem.md), que indica que são itens de uma unidade diferente. Para acessar o recurso compartilhado DriveItem, você precisará fazer uma solicitação usando as informações fornecidas em **remoteItem** no seguinte formato:</span><span class="sxs-lookup"><span data-stu-id="af88c-p104">DriveItems returned from the **sharedWithMe** action will always include the [**remoteItem**](../resources/remoteitem.md) facet which indicates they are items from a different drive. To access the shared DriveItem resource, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<span data-ttu-id="af88c-131">Por padrão, **sharedWithMe** retorna itens compartilhados no seu próprio locatário.</span><span class="sxs-lookup"><span data-stu-id="af88c-131">By default, **sharedWithMe** return items shared within your own tenant.</span></span> <span data-ttu-id="af88c-132">Para incluir itens compartilhados de locatários externos, acrescente `?allowexternal=true` à solicitação GET.</span><span class="sxs-lookup"><span data-stu-id="af88c-132">To include items shared from external tenants, append `?allowexternal=true` to the GET request.</span></span>



<!-- {
  "type": "#page.annotation",
  "description": "List the items shared with the owner of a drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Sharing/Shared with me",
  "suppressions": [
  ]
} -->
