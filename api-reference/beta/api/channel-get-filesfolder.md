---
title: Obter filesFolder
description: Recupere o caminho de navegação do filesFolder de um canal.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: be54dc5e25d84fa9cd6c70faf926a8708ce9c475
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863111"
---
# <a name="get-filesfolder"></a><span data-ttu-id="21bff-103">Obter filesFolder</span><span class="sxs-lookup"><span data-stu-id="21bff-103">Get filesFolder</span></span>

<span data-ttu-id="21bff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21bff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21bff-105">Obter os metadados para o local onde os arquivos de um [canal](../resources/channel.md) estão armazenados.</span><span class="sxs-lookup"><span data-stu-id="21bff-105">Get the metadata for the location where the files of a [channel](../resources/channel.md) are stored.</span></span> 

## <a name="permissions"></a><span data-ttu-id="21bff-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="21bff-106">Permissions</span></span>
<span data-ttu-id="21bff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21bff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21bff-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21bff-109">Permission type</span></span>      | <span data-ttu-id="21bff-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21bff-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21bff-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21bff-111">Delegated (work or school account)</span></span> | <span data-ttu-id="21bff-112">File. Read. All, Group. Read. All, File. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="21bff-112">File.Read.All, Group.Read.All, File.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="21bff-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21bff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21bff-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21bff-114">Not supported.</span></span>    |
|<span data-ttu-id="21bff-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21bff-115">Application</span></span> | <span data-ttu-id="21bff-116">File. Read. All, Group. Read. All, File. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="21bff-116">File.Read.All, Group.Read.All, File.ReadWrite.All, Group.ReadWrite.All</span></span>     |


## <a name="http-request"></a><span data-ttu-id="21bff-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21bff-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/filesFolder

```

## <a name="optional-query-parameters"></a><span data-ttu-id="21bff-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="21bff-118">Optional query parameters</span></span>

<span data-ttu-id="21bff-119">Este método não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="21bff-119">This method does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="21bff-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21bff-120">Request headers</span></span>
| <span data-ttu-id="21bff-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21bff-121">Header</span></span>       | <span data-ttu-id="21bff-122">Valor</span><span class="sxs-lookup"><span data-stu-id="21bff-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="21bff-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="21bff-123">Authorization</span></span>  | <span data-ttu-id="21bff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21bff-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="21bff-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21bff-126">Request body</span></span>
<span data-ttu-id="21bff-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="21bff-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21bff-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="21bff-128">Response</span></span>

<span data-ttu-id="21bff-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [driveItem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21bff-129">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21bff-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21bff-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="21bff-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21bff-131">Request</span></span>
<span data-ttu-id="21bff-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="21bff-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="21bff-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="21bff-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_filesFolder"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/filesFolder
```
# <a name="c"></a>[<span data-ttu-id="21bff-134">C#</span><span class="sxs-lookup"><span data-stu-id="21bff-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-filesfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21bff-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21bff-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-filesfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21bff-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21bff-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-filesfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="21bff-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="21bff-137">Response</span></span>
<span data-ttu-id="21bff-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="21bff-138">The following is an example of the response.</span></span> 

><span data-ttu-id="21bff-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21bff-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('32e3b156-66b2-4135-9aeb-73295a35a55b')/channels('19%3Af253e46c035b42308e9a4a22a87037af%40thread.skype')/filesFolder/$entity",
    "id": "01H7CFEKENJSSIUHGADZBKODARINQC5JMD",
    "createdDateTime": "0001-01-01T00:00:00Z",
    "lastModifiedDateTime": "2020-01-23T18:47:13Z",
    "name": "Documentation Planning",
    "webUrl": "https://microsoft.sharepoint.com/teams/ExtensibilityandFundamentals/Shared%20Documents/Documentation%20Planning",
    "size": 2374080,
    "parentReference": {
        "driveId": "b!2SInBlQrN0K8-GXMy9qNsPtI5ScW8C5IlZtycoy6ZpJZRRtgE4qVTrE8wrvL0-hd",
        "driveType": "documentLibrary"
    },
    "fileSystemInfo": {
        "createdDateTime": "2020-01-23T18:47:12Z",
        "lastModifiedDateTime": "2020-01-23T18:47:13Z"
    },
    "folder": {
        "childCount": 7
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get filesFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

