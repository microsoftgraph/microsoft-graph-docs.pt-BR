---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Copiar um arquivo ou pasta
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: cdb22395cfde6820eb5450f39bd1e3408a4f82b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454558"
---
# <a name="copy-a-driveitem"></a><span data-ttu-id="1947f-102">Copiar um DriveItem</span><span class="sxs-lookup"><span data-stu-id="1947f-102">Copy a DriveItem</span></span>

<span data-ttu-id="1947f-103">Cria uma cópia de forma assíncrona de um [driveItem][item-resource] (incluindo os filhos), em um novo item pai ou com um novo nome.</span><span class="sxs-lookup"><span data-stu-id="1947f-103">Asynchronously creates a copy of an [driveItem][item-resource] (including any children), under a new parent item or with a new name.</span></span>

## <a name="permissions"></a><span data-ttu-id="1947f-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="1947f-104">Permissions</span></span>

<span data-ttu-id="1947f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1947f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1947f-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1947f-107">Permission type</span></span>      | <span data-ttu-id="1947f-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1947f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1947f-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1947f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="1947f-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1947f-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1947f-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1947f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1947f-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1947f-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="1947f-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1947f-113">Application</span></span> | <span data-ttu-id="1947f-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1947f-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1947f-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1947f-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

### <a name="request-body"></a><span data-ttu-id="1947f-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1947f-116">Request body</span></span>

<span data-ttu-id="1947f-117">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1947f-117">In the request body, provide a JSON object with the following parameters.</span></span>


| <span data-ttu-id="1947f-118">Name</span><span class="sxs-lookup"><span data-stu-id="1947f-118">Name</span></span>            | <span data-ttu-id="1947f-119">Valor</span><span class="sxs-lookup"><span data-stu-id="1947f-119">Value</span></span>                                          | <span data-ttu-id="1947f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1947f-120">Description</span></span>                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1947f-121">parentReference</span><span class="sxs-lookup"><span data-stu-id="1947f-121">parentReference</span></span> | [<span data-ttu-id="1947f-122">ItemReference</span><span class="sxs-lookup"><span data-stu-id="1947f-122">ItemReference</span></span>](../resources/itemreference.md) | <span data-ttu-id="1947f-p102">Opcional. Referência ao item pai em que a cópia será criada.</span><span class="sxs-lookup"><span data-stu-id="1947f-p102">Optional. Reference to the parent item the copy will be created in.</span></span>                                         |
| <span data-ttu-id="1947f-125">nome</span><span class="sxs-lookup"><span data-stu-id="1947f-125">name</span></span>            | <span data-ttu-id="1947f-126">string</span><span class="sxs-lookup"><span data-stu-id="1947f-126">string</span></span>                                         | <span data-ttu-id="1947f-p103">Opcional. O novo nome para a cópia. Se isso não for fornecido, será usado o mesmo nome que o original.</span><span class="sxs-lookup"><span data-stu-id="1947f-p103">Optional. The new name for the copy. If this isn't provided, the same name will be used as the original.</span></span>    |

<span data-ttu-id="1947f-130">**Observação:** _parentReference_ deve incluir os parâmetros `driveId` e `id` para a pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="1947f-130">**Note:** The _parentReference_ should include the `driveId` and `id` parameters for the target folder.</span></span>

## <a name="example"></a><span data-ttu-id="1947f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1947f-131">Example</span></span>

<span data-ttu-id="1947f-132">Este exemplo copia um arquivo identificado por `{item-id}` em uma pasta identificada por um valor `driveId` e `id`.</span><span class="sxs-lookup"><span data-stu-id="1947f-132">This example copies a file identified by `{item-id}` into a folder identified with a `driveId` and `id` value.</span></span>
<span data-ttu-id="1947f-133">A nova cópia do arquivo será nomeada `contoso plan (copy).txt`.</span><span class="sxs-lookup"><span data-stu-id="1947f-133">The new copy of the file will be named `contoso plan (copy).txt`.</span></span>

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

## <a name="response"></a><span data-ttu-id="1947f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1947f-134">Response</span></span>

<span data-ttu-id="1947f-135">Retorna detalhes sobre como [monitorar o progresso](/graph/long-running-actions-overview) da cópia após aceitar a solicitação.</span><span class="sxs-lookup"><span data-stu-id="1947f-135">Returns details about how to [monitor the progress](/graph/long-running-actions-overview) of the copy, upon accepting the request.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="1947f-p105">O valor do cabeçalho `Location` fornece uma URL para um serviço que irá retornar o estado atual da operação de cópia. Você pode usar essas informações para [determinar quando a cópia terminou](/graph/long-running-actions-overview).</span><span class="sxs-lookup"><span data-stu-id="1947f-p105">The value of the `Location` header provides a URL for a service that will return the current state of the copy operation. You can use this info to [determine when the copy has finished](/graph/long-running-actions-overview).</span></span>

### <a name="remarks"></a><span data-ttu-id="1947f-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="1947f-138">Remarks</span></span>

<span data-ttu-id="1947f-p106">Em muitos casos, a ação de copiar é executada de forma assíncrona. A resposta da API só indicará que a operação de cópia foi aceita ou rejeitada, por exemplo, porque o nome de arquivo de destino já está sendo utilizado.</span><span class="sxs-lookup"><span data-stu-id="1947f-p106">In many cases the copy action is performed asynchronously. The response from the API will only indicate that the copy operation was accepted or rejected, say due to the destination filename already being in use.</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
