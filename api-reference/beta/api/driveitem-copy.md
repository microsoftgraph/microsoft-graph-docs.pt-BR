---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Copiar um arquivo ou uma pasta
localization_priority: Normal
ms.openlocfilehash: 8289bd3c15575e1469fe18baf45c6c2f937ed2dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879440"
---
# <a name="copy-a-driveitem"></a><span data-ttu-id="5c1e8-102">Copiar um DriveItem</span><span class="sxs-lookup"><span data-stu-id="5c1e8-102">Copy a DriveItem</span></span>

> <span data-ttu-id="5c1e8-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5c1e8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c1e8-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5c1e8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5c1e8-105">Cria uma cópia de forma assíncrona de um [driveItem][item-resource] (incluindo os filhos), em um novo item pai ou com um novo nome.</span><span class="sxs-lookup"><span data-stu-id="5c1e8-105">Asynchronously creates a copy of an [driveItem][item-resource] (including any children), under a new parent item or with a new name.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c1e8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c1e8-106">Permissions</span></span>

<span data-ttu-id="5c1e8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c1e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c1e8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c1e8-109">Permission type</span></span>      | <span data-ttu-id="5c1e8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c1e8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c1e8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c1e8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5c1e8-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c1e8-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5c1e8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c1e8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c1e8-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c1e8-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="5c1e8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c1e8-115">Application</span></span> | <span data-ttu-id="5c1e8-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c1e8-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c1e8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c1e8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

### <a name="request-body"></a><span data-ttu-id="5c1e8-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c1e8-118">Request body</span></span>

<span data-ttu-id="5c1e8-119">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c1e8-119">In the request body, provide a JSON object with the following parameters.</span></span>


| <span data-ttu-id="5c1e8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5c1e8-120">Name</span></span>            | <span data-ttu-id="5c1e8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5c1e8-121">Value</span></span>                                          | <span data-ttu-id="5c1e8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c1e8-122">Description</span></span>                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5c1e8-123">parentReference</span><span class="sxs-lookup"><span data-stu-id="5c1e8-123">parentReference</span></span> | [<span data-ttu-id="5c1e8-124">ItemReference</span><span class="sxs-lookup"><span data-stu-id="5c1e8-124">ItemReference</span></span>](../resources/itemreference.md) | <span data-ttu-id="5c1e8-p103">Opcional. Referência ao item pai em que a cópia será criada.</span><span class="sxs-lookup"><span data-stu-id="5c1e8-p103">Optional. Reference to the parent item the copy will be created in.</span></span>                                         |
| <span data-ttu-id="5c1e8-127">name</span><span class="sxs-lookup"><span data-stu-id="5c1e8-127">name</span></span>            | <span data-ttu-id="5c1e8-128">string</span><span class="sxs-lookup"><span data-stu-id="5c1e8-128">string</span></span>                                         | <span data-ttu-id="5c1e8-p104">Opcional. O novo nome para a cópia. Se isso não for fornecido, será usado o mesmo nome que o original.</span><span class="sxs-lookup"><span data-stu-id="5c1e8-p104">Optional. The new name for the copy. If this isn't provided, the same name will be used as the original.</span></span>    |

<span data-ttu-id="5c1e8-132">**Observação:** _parentReference_ deve incluir os parâmetros `driveId` e `id` para a pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="5c1e8-132">**Note:** The _parentReference_ should include the `driveId` and `id` parameters for the target folder.</span></span>

## <a name="example"></a><span data-ttu-id="5c1e8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c1e8-133">Example</span></span>

<span data-ttu-id="5c1e8-134">Este exemplo copia um arquivo identificado por `{item-id}` em uma pasta identificada por um valor `driveId` e `id`.</span><span class="sxs-lookup"><span data-stu-id="5c1e8-134">This example copies a file identified by `{item-id}` into a folder identified with a `driveId` and `id` value.</span></span>
<span data-ttu-id="5c1e8-135">A nova cópia do arquivo será nomeada `contoso plan (copy).txt`.</span><span class="sxs-lookup"><span data-stu-id="5c1e8-135">The new copy of the file will be named `contoso plan (copy).txt`.</span></span>

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

## <a name="response"></a><span data-ttu-id="5c1e8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c1e8-136">Response</span></span>

<span data-ttu-id="5c1e8-137">Retorna detalhes sobre como [monitorar o progresso](/graph/long-running-actions-overview) da cópia após aceitar a solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c1e8-137">Returns details about how to [monitor the progress](/graph/long-running-actions-overview) of the copy, upon accepting the request.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="5c1e8-138">O valor do cabeçalho `Location` fornece uma URL para um serviço que irá retornar o estado atual da operação de cópia.</span><span class="sxs-lookup"><span data-stu-id="5c1e8-138">The value of the `Location` header provides a URL for a service that will return the current state of the copy operation.</span></span>
<span data-ttu-id="5c1e8-139">Você pode usar essas informações para [determinar quando a cópia terminou](/graph/long-running-actions-overview).</span><span class="sxs-lookup"><span data-stu-id="5c1e8-139">You can use this info to [determine when the copy has finished](/graph/long-running-actions-overview).</span></span>

### <a name="remarks"></a><span data-ttu-id="5c1e8-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="5c1e8-140">Remarks</span></span>

<span data-ttu-id="5c1e8-p107">Em muitos casos, a ação de copiar é executada de forma assíncrona. A resposta da API só indicará que a operação de cópia foi aceita ou rejeitada, por exemplo, porque o nome de arquivo de destino já está sendo utilizado.</span><span class="sxs-lookup"><span data-stu-id="5c1e8-p107">In many cases the copy action is performed asynchronously. The response from the API will only indicate that the copy operation was accepted or rejected, say due to the destination filename already being in use.</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
