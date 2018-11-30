---
author: chackman
ms.author: chackman
title: Listar itens visitados
ms.openlocfilehash: dfaa727d25b3713d1be2a8d49f87dab8dba3b553
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038048"
---
# <a name="list-followed-items"></a><span data-ttu-id="af368-102">Listar itens visitados</span><span class="sxs-lookup"><span data-stu-id="af368-102">List followed items</span></span>

> <span data-ttu-id="af368-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="af368-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af368-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="af368-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="af368-105">Lista os [itens](../resources/driveitem.md) que foram visitados pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="af368-105">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="af368-106">Esta coleção inclui itens que estão na unidade do usuário, bem como os itens que eles têm acesso a partir de outras unidades.</span><span class="sxs-lookup"><span data-stu-id="af368-106">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="af368-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="af368-107">Permissions</span></span>

<span data-ttu-id="af368-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af368-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af368-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af368-110">Permission type</span></span>      | <span data-ttu-id="af368-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af368-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af368-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af368-112">Delegated (work or school account)</span></span> | <span data-ttu-id="af368-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af368-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="af368-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af368-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af368-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af368-115">Not supported.</span></span>    |
|<span data-ttu-id="af368-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af368-116">Application</span></span> | <span data-ttu-id="af368-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af368-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="af368-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af368-118">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```

## <a name="response"></a><span data-ttu-id="af368-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="af368-119">Response</span></span>

<span data-ttu-id="af368-120">Esse método retorna uma coleção de recursos de [driveItem](../resources/driveitem.md) para itens que o proprietário da unidade está seguindo.</span><span class="sxs-lookup"><span data-stu-id="af368-120">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="af368-121">Se nenhum item foi encontrado, uma coleção vazia é retornada.</span><span class="sxs-lookup"><span data-stu-id="af368-121">If no items were found, an empty collection is returned.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "name": "March Proposal.docx",
      "size": 19121,
      "lastModifiedDateTime": "2017-12-12T10:40:59Z"
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "size": 37810,
      "lastModifiedDateTime": "2016-10-18T10:40:59Z"
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List the items a user is following.",
  "keywords": "drive,onedrive.drive,list followed items",
  "section": "documentation",
  "tocPath": "Drives/List followed items"
} -->
