---
title: Obter filesFolder
description: Recuperar o filesFolder do caminho de navegação de um canal.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9af36b403733b0f0937210b5c959b7203e8deef7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959287"
---
# <a name="get-filesfolder"></a><span data-ttu-id="c8650-103">Obter filesFolder</span><span class="sxs-lookup"><span data-stu-id="c8650-103">Get filesFolder</span></span>

<span data-ttu-id="c8650-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8650-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8650-105">Obter os metadados para o local em que os arquivos do [canal](../resources/channel.md) estão armazenados.</span><span class="sxs-lookup"><span data-stu-id="c8650-105">Get the metadata for the location where the files of a [channel](../resources/channel.md) are stored.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c8650-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c8650-106">Permissions</span></span>
<span data-ttu-id="c8650-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8650-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8650-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8650-109">Permission type</span></span>      | <span data-ttu-id="c8650-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c8650-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8650-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8650-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c8650-112">Files.Read.All, Files.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8650-112">Files.Read.All, Files.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="c8650-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8650-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8650-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8650-114">Not supported.</span></span>    |
|<span data-ttu-id="c8650-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8650-115">Application</span></span> | <span data-ttu-id="c8650-116">Files.Read.All, Files.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8650-116">Files.Read.All, Files.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="c8650-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8650-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/filesFolder
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8650-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c8650-118">Optional query parameters</span></span>

<span data-ttu-id="c8650-119">Este método não é compatível com os [Parâmetros de Consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c8650-119">This method does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8650-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8650-120">Request headers</span></span>
| <span data-ttu-id="c8650-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c8650-121">Header</span></span>       | <span data-ttu-id="c8650-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c8650-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c8650-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8650-123">Authorization</span></span>  | <span data-ttu-id="c8650-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8650-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c8650-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8650-126">Request body</span></span>
<span data-ttu-id="c8650-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c8650-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8650-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8650-128">Response</span></span>

<span data-ttu-id="c8650-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [driveItem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8650-129">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8650-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8650-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="c8650-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8650-131">Request</span></span>
<span data-ttu-id="c8650-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8650-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c8650-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8650-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_filesFolder"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/filesFolder
```
# <a name="c"></a>[<span data-ttu-id="c8650-134">C#</span><span class="sxs-lookup"><span data-stu-id="c8650-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-filesfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8650-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8650-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-filesfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8650-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8650-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-filesfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c8650-137">Java</span><span class="sxs-lookup"><span data-stu-id="c8650-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-filesfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c8650-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8650-138">Response</span></span>
<span data-ttu-id="c8650-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c8650-139">The following is an example of the response.</span></span> 

><span data-ttu-id="c8650-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8650-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "lastEditedDateTime": null,
    "name": "Documentation Planning",
    "webUrl": "https://microsoft.sharepoint.com/teams/ExtensibilityandFundamentals/Shared%20Documents/Documentation%20Planning",
    "size": 2374080,
    "parentReference": {
        "driveId": "b!2SInBlQrN0K8-GXMy9qNsPtI5ScW8C5IlZtycoy6ZpJZRRtgE4qVTrE8wrvL0-hd",
        "driveType": "documentLibrary"
    },
    "fileSystemInfo": {
        "createdDateTime": "2020-01-23T18:47:12Z",
        "lastModifiedDateTime": "2020-01-23T18:47:13Z",
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



