---
author: JeremyKelley
ms.date: 09/10/2017
title: Copiar um arquivo ou pasta
localization_priority: Normal
ms.prod: sharepoint
description: Cria uma cópia de forma assíncrona de um driveItem (incluindo os filhos), em um novo item pai ou com um novo nome.
doc_type: apiPageType
ms.openlocfilehash: 697f52cae983802af2a6c0a2bf39774873f82e46
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239594"
---
# <a name="copy-a-driveitem"></a><span data-ttu-id="5b831-103">Copiar um DriveItem</span><span class="sxs-lookup"><span data-stu-id="5b831-103">Copy a DriveItem</span></span>

<span data-ttu-id="5b831-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b831-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5b831-105">Cria uma cópia de forma assíncrona de um [driveItem][item-resource] (incluindo os filhos), em um novo item pai ou com um novo nome.</span><span class="sxs-lookup"><span data-stu-id="5b831-105">Asynchronously creates a copy of an [driveItem][item-resource] (including any children), under a new parent item or with a new name.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b831-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b831-106">Permissions</span></span>

<span data-ttu-id="5b831-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b831-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b831-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b831-109">Permission type</span></span>      | <span data-ttu-id="5b831-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b831-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b831-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b831-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5b831-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b831-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5b831-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b831-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b831-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b831-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="5b831-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b831-115">Application</span></span> | <span data-ttu-id="5b831-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b831-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b831-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b831-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

### <a name="request-body"></a><span data-ttu-id="5b831-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b831-118">Request body</span></span>

<span data-ttu-id="5b831-119">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b831-119">In the request body, provide a JSON object with the following parameters.</span></span>


| <span data-ttu-id="5b831-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5b831-120">Name</span></span>            | <span data-ttu-id="5b831-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5b831-121">Value</span></span>                                          | <span data-ttu-id="5b831-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b831-122">Description</span></span>                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5b831-123">parentReference</span><span class="sxs-lookup"><span data-stu-id="5b831-123">parentReference</span></span> | [<span data-ttu-id="5b831-124">ItemReference</span><span class="sxs-lookup"><span data-stu-id="5b831-124">ItemReference</span></span>](../resources/itemreference.md) | <span data-ttu-id="5b831-p102">Opcional. Referência ao item pai em que a cópia será criada.</span><span class="sxs-lookup"><span data-stu-id="5b831-p102">Optional. Reference to the parent item the copy will be created in.</span></span>                                         |
| <span data-ttu-id="5b831-127">name</span><span class="sxs-lookup"><span data-stu-id="5b831-127">name</span></span>            | <span data-ttu-id="5b831-128">string</span><span class="sxs-lookup"><span data-stu-id="5b831-128">string</span></span>                                         | <span data-ttu-id="5b831-p103">Opcional. O novo nome para a cópia. Se isso não for fornecido, será usado o mesmo nome que o original.</span><span class="sxs-lookup"><span data-stu-id="5b831-p103">Optional. The new name for the copy. If this isn't provided, the same name will be used as the original.</span></span>    |

<span data-ttu-id="5b831-132">**Observação:** _parentReference_ deve incluir os parâmetros `driveId` e `id` para a pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="5b831-132">**Note:** The _parentReference_ should include the `driveId` and `id` parameters for the target folder.</span></span>

## <a name="example"></a><span data-ttu-id="5b831-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b831-133">Example</span></span>

<span data-ttu-id="5b831-134">Este exemplo copia um arquivo identificado por `{item-id}` em uma pasta identificada por um valor `driveId` e `id`.</span><span class="sxs-lookup"><span data-stu-id="5b831-134">This example copies a file identified by `{item-id}` into a folder identified with a `driveId` and `id` value.</span></span>
<span data-ttu-id="5b831-135">A nova cópia do arquivo será nomeada `contoso plan (copy).txt`.</span><span class="sxs-lookup"><span data-stu-id="5b831-135">The new copy of the file will be named `contoso plan (copy).txt`.</span></span>


# <a name="http"></a>[<span data-ttu-id="5b831-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b831-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite", "tags": "service.graph", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "driveId": "6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B",
    "id": "DCD0D3AD-8989-4F23-A5A2-2C086050513F"
  },
  "name": "contoso plan (copy).txt"
}
```
# <a name="c"></a>[<span data-ttu-id="5b831-137">C#</span><span class="sxs-lookup"><span data-stu-id="5b831-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/copy-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b831-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b831-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/copy-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b831-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b831-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/copy-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5b831-140">Java</span><span class="sxs-lookup"><span data-stu-id="5b831-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/copy-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="5b831-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b831-141">Response</span></span>

<span data-ttu-id="5b831-142">Retorna detalhes sobre como [monitorar o progresso](/graph/long-running-actions-overview) da cópia após aceitar a solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b831-142">Returns details about how to [monitor the progress](/graph/long-running-actions-overview) of the copy, upon accepting the request.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="5b831-p105">O valor do cabeçalho `Location` fornece uma URL para um serviço que irá retornar o estado atual da operação de cópia. Você pode usar essas informações para [determinar quando a cópia terminou](/graph/long-running-actions-overview).</span><span class="sxs-lookup"><span data-stu-id="5b831-p105">The value of the `Location` header provides a URL for a service that will return the current state of the copy operation. You can use this info to [determine when the copy has finished](/graph/long-running-actions-overview).</span></span>

### <a name="remarks"></a><span data-ttu-id="5b831-145">Comentários</span><span class="sxs-lookup"><span data-stu-id="5b831-145">Remarks</span></span>

<span data-ttu-id="5b831-p106">Em muitos casos, a ação de copiar é executada de forma assíncrona. A resposta da API só indicará que a operação de cópia foi aceita ou rejeitada, por exemplo, porque o nome de arquivo de destino já está sendo utilizado.</span><span class="sxs-lookup"><span data-stu-id="5b831-p106">In many cases the copy action is performed asynchronously. The response from the API will only indicate that the copy operation was accepted or rejected, say due to the destination filename already being in use.</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
} -->

