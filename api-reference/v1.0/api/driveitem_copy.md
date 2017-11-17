---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Copiar um arquivo ou uma pasta
ms.openlocfilehash: 6740091f887e42a14b2a42c99ee586af4254c473
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="copy-a-driveitem"></a><span data-ttu-id="25724-102">Copiar um DriveItem</span><span class="sxs-lookup"><span data-stu-id="25724-102">Copy a DriveItem</span></span>

<span data-ttu-id="25724-103">Cria uma cópia de forma assíncrona de um [driveItem][item-resource] (incluindo os filhos), em um novo item pai ou com um novo nome.</span><span class="sxs-lookup"><span data-stu-id="25724-103">Creates a copy of a [driveItem] (including any children) under a new parent or with a new name.</span></span>

## <a name="permissions"></a><span data-ttu-id="25724-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="25724-104">Permissions</span></span>

<span data-ttu-id="25724-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="25724-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="25724-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25724-107">Permission type</span></span>      | <span data-ttu-id="25724-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25724-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25724-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25724-109">Delegated (work or school account)</span></span> | <span data-ttu-id="25724-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25724-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="25724-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25724-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25724-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25724-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="25724-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25724-113">Application</span></span> | <span data-ttu-id="25724-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25724-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="25724-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25724-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

### <a name="request-body"></a><span data-ttu-id="25724-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25724-116">Request body</span></span>

<span data-ttu-id="25724-117">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25724-117">In the request body, provide a JSON object with the following parameters.</span></span>


| <span data-ttu-id="25724-118">Nome</span><span class="sxs-lookup"><span data-stu-id="25724-118">Name</span></span>            | <span data-ttu-id="25724-119">Valor</span><span class="sxs-lookup"><span data-stu-id="25724-119">Value</span></span>                                          | <span data-ttu-id="25724-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="25724-120">Description</span></span>                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="25724-121">parentReference</span><span class="sxs-lookup"><span data-stu-id="25724-121">parentReference</span></span> | [<span data-ttu-id="25724-122">ItemReference</span><span class="sxs-lookup"><span data-stu-id="25724-122">ItemReference</span></span>](../resources/itemreference.md) | <span data-ttu-id="25724-p102">Opcional. Referência ao item pai em que a cópia será criada.</span><span class="sxs-lookup"><span data-stu-id="25724-p102">Optional. Reference to the parent item the copy will be created in.</span></span>                                         |
| <span data-ttu-id="25724-125">name</span><span class="sxs-lookup"><span data-stu-id="25724-125">name</span></span>            | <span data-ttu-id="25724-126">string</span><span class="sxs-lookup"><span data-stu-id="25724-126">string</span></span>                                         | <span data-ttu-id="25724-p103">Opcional. O novo nome para a cópia. Se isso não for fornecido, será usado o mesmo nome que o original.</span><span class="sxs-lookup"><span data-stu-id="25724-p103">Optional. The new name for the copy. If this isn't provided, the same name will be used as the original.</span></span>    |

<span data-ttu-id="25724-130">**Observação:** _parentReference_ deve incluir os parâmetros `driveId` e `id` para a pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="25724-130">**Note:** The _parentReference_ should include the `driveId` and `id` parameters for the target folder.</span></span>

## <a name="example"></a><span data-ttu-id="25724-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25724-131">Example</span></span>

<span data-ttu-id="25724-132">Este exemplo copia um arquivo identificado por `{item-id}` em uma pasta identificada por um valor `driveId` e `id`.</span><span class="sxs-lookup"><span data-stu-id="25724-132">This example copies a file identified by `{item-id}` into a folder identified with a `driveId` and `id` value.</span></span>
<span data-ttu-id="25724-133">A nova cópia do arquivo será nomeada `contoso plan (copy).txt`.</span><span class="sxs-lookup"><span data-stu-id="25724-133">The new copy of the file will be named `contoso plan (copy).txt`.</span></span>

<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite", "target": "action" } -->

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

## <a name="response"></a><span data-ttu-id="25724-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="25724-134">Response</span></span>

<span data-ttu-id="25724-135">Retorna detalhes sobre como [monitorar o progresso](../../../concepts/long_running_actions_overview.md) da cópia após aceitar a solicitação.</span><span class="sxs-lookup"><span data-stu-id="25724-135">Returns details about how to [monitor the progress](../../../concepts/long_running_actions_overview.md) of the copy, upon accepting the request.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="25724-136">O valor do cabeçalho `Location` fornece uma URL para um serviço que irá retornar o estado atual da operação de cópia.</span><span class="sxs-lookup"><span data-stu-id="25724-136">The value of the `Location` header provides a URL for a service that will return the current state of the copy operation.</span></span>
<span data-ttu-id="25724-137">Você pode usar essas informações para [determinar quando a cópia terminou](../../../concepts/long_running_actions_overview.md).</span><span class="sxs-lookup"><span data-stu-id="25724-137">You can use this info to [determine when the copy has finished](../../../concepts/long_running_actions_overview.md).</span></span>

### <a name="remarks"></a><span data-ttu-id="25724-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="25724-138">Remarks</span></span>

<span data-ttu-id="25724-p106">Em muitos casos, a ação de copiar é executada de forma assíncrona. A resposta da API só indicará que a operação de cópia foi aceita ou rejeitada, por exemplo, porque o nome de arquivo de destino já está sendo utilizado.</span><span class="sxs-lookup"><span data-stu-id="25724-p106">In many cases the copy action is performed asynchronously. The response from the API will only indicate that the copy operation was accepted or rejected, say due to the destination filename already being in use.</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
