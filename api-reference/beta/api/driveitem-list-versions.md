---
title: Listando versões de um DriveItem
description: O OneDrive e o SharePoint podem ser configurados para manter o histórico de arquivos.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 52df6b0f7e452d358160de886ed61824fd2d48d0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915722"
---
# <a name="listing-versions-of-a-driveitem"></a><span data-ttu-id="0eddc-103">Listando versões de um DriveItem</span><span class="sxs-lookup"><span data-stu-id="0eddc-103">Listing versions of a DriveItem</span></span>

> <span data-ttu-id="0eddc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0eddc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0eddc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0eddc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0eddc-106">O OneDrive e o SharePoint podem ser configurados para manter o histórico de arquivos.</span><span class="sxs-lookup"><span data-stu-id="0eddc-106">OneDrive and SharePoint can be configured to retain the history for files.</span></span>
<span data-ttu-id="0eddc-107">Dependendo do serviço e da configuração, uma nova versão pode ser criada para cada edição, sempre que o arquivo for salvo, manualmente ou nunca.</span><span class="sxs-lookup"><span data-stu-id="0eddc-107">Depending on the service and configuration, a new version can be created for each edit, each time the file is saved, manually, or never.</span></span>

<span data-ttu-id="0eddc-108">Versões anteriores de um documento podem ser retidas por um determinado período dependendo das configurações de administração, que podem ser exclusivas por usuário ou local.</span><span class="sxs-lookup"><span data-stu-id="0eddc-108">Previous versions of a document may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="0eddc-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="0eddc-109">Permissions</span></span>

<span data-ttu-id="0eddc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0eddc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0eddc-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0eddc-112">Permission type</span></span>      | <span data-ttu-id="0eddc-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0eddc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0eddc-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0eddc-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0eddc-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eddc-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0eddc-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0eddc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0eddc-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eddc-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="0eddc-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0eddc-118">Application</span></span> | <span data-ttu-id="0eddc-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eddc-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="0eddc-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0eddc-120">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions
GET /groups/{group-id}/drive/{item-id}/versions
GET /me/drive/items/{item-id}/versions
GET /sites/{site-id}/drive/items/{item-id}/versions
GET /users/{user-id}/drive/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="0eddc-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="0eddc-121">Response</span></span>

<span data-ttu-id="0eddc-122">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [DriveItemVersion](../resources/driveitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0eddc-122">If successful, this method returns a `200 OK` response code and collection of [DriveItemVersion](../resources/driveitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="0eddc-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0eddc-123">Example</span></span>

<span data-ttu-id="0eddc-124">Este exemplo recupera as versões de um arquivo na unidade do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="0eddc-124">This example retrieves the versions of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="0eddc-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0eddc-125">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="0eddc-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0eddc-126">Response</span></span>

<span data-ttu-id="0eddc-127">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="0eddc-127">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
      "size": 123
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z",
      "size": 62
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z",
      "size": 16
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="0eddc-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="0eddc-128">Remarks</span></span>

<span data-ttu-id="0eddc-129">O OneDrive não preserva os metadados completos de versões anteriores de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="0eddc-129">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="0eddc-130">Quando seu aplicativo recupera a lista de versões disponíveis de um arquivo, um recurso [DriveItemVersion](../resources/driveitemversion.md) é retornado e fornece as informações disponíveis sobre a versão específica.</span><span class="sxs-lookup"><span data-stu-id="0eddc-130">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
