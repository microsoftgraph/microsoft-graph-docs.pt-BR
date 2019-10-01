---
title: 'driveItem: restaurar'
description: Restaurar um driveItem que foi excluído e que está atualmente na lixeira.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
ms.date: 08/06/2019
doc_type: apiPageType
ms.openlocfilehash: 501b18272811e7de35971ec9cc325772f080e2ea
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333378"
---
# <a name="driveitem-restore"></a><span data-ttu-id="4e59f-103">driveItem: restaurar</span><span class="sxs-lookup"><span data-stu-id="4e59f-103">driveItem: restore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e59f-104">Restaurar um [driveItem](../resources/driveitem.md) que foi excluído e que está atualmente na lixeira.</span><span class="sxs-lookup"><span data-stu-id="4e59f-104">Restore a [driveItem](../resources/driveitem.md) that has been deleted and is currently in the recycle bin.</span></span> <span data-ttu-id="4e59f-105">**Observação**: atualmente, essa funcionalidade só está disponível para o onedrive Personal.</span><span class="sxs-lookup"><span data-stu-id="4e59f-105">**NOTE**: This functionality is currently only available for OneDrive Personal.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e59f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4e59f-106">Permissions</span></span>

<span data-ttu-id="4e59f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e59f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4e59f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e59f-109">Permission type</span></span>                        | <span data-ttu-id="4e59f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4e59f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4e59f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e59f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4e59f-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e59f-112">Not supported.</span></span> |
| <span data-ttu-id="4e59f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e59f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e59f-114">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e59f-114">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="4e59f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e59f-115">Application</span></span>                            | <span data-ttu-id="4e59f-116">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e59f-116">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e59f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e59f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/drive/items/{item-id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="4e59f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e59f-118">Request headers</span></span>

| <span data-ttu-id="4e59f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4e59f-119">Name</span></span>          | <span data-ttu-id="4e59f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e59f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4e59f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e59f-121">Authorization</span></span> | <span data-ttu-id="4e59f-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="4e59f-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e59f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e59f-123">Request body</span></span>

<span data-ttu-id="4e59f-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e59f-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4e59f-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4e59f-125">Parameter</span></span>     | <span data-ttu-id="4e59f-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e59f-126">Type</span></span>                                         | <span data-ttu-id="4e59f-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e59f-127">Description</span></span> |
|:--------------|:---------------------------------------------|:------------|
|<span data-ttu-id="4e59f-128">parentReference</span><span class="sxs-lookup"><span data-stu-id="4e59f-128">parentReference</span></span>|[<span data-ttu-id="4e59f-129">ItemReference</span><span class="sxs-lookup"><span data-stu-id="4e59f-129">ItemReference</span></span>](../resources/itemreference.md)| <span data-ttu-id="4e59f-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="4e59f-130">Optional.</span></span> <span data-ttu-id="4e59f-131">Referência ao item pai no qual o item excluído será restaurado.</span><span class="sxs-lookup"><span data-stu-id="4e59f-131">Reference to the parent item the deleted item will be restored to.</span></span> |
|<span data-ttu-id="4e59f-132">name</span><span class="sxs-lookup"><span data-stu-id="4e59f-132">name</span></span>           |<span data-ttu-id="4e59f-133">String</span><span class="sxs-lookup"><span data-stu-id="4e59f-133">String</span></span>                                        | <span data-ttu-id="4e59f-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="4e59f-134">Optional.</span></span> <span data-ttu-id="4e59f-135">O novo nome do item restaurado.</span><span class="sxs-lookup"><span data-stu-id="4e59f-135">The new name for the restored item.</span></span> <span data-ttu-id="4e59f-136">Se isso não for fornecido, será usado o mesmo nome que o original.</span><span class="sxs-lookup"><span data-stu-id="4e59f-136">If this isn't provided, the same name will be used as the original.</span></span> |

## <a name="response"></a><span data-ttu-id="4e59f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e59f-137">Response</span></span>

<span data-ttu-id="4e59f-138">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [driveItem](../resources/driveitem.md) restaurado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e59f-138">If successful, this method returns `200 OK` response code and the restored [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4e59f-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4e59f-139">Examples</span></span>

<span data-ttu-id="4e59f-140">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="4e59f-140">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="4e59f-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e59f-141">Request</span></span>

<span data-ttu-id="4e59f-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e59f-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "restore-item",
  "scopes": "files.readwrite",
  "target": "action"
}-->

```http
POST https://graph.microsoft.com/beta/me/drive/items/{item-id}/restore
Content-type: application/json

{
  "parentReference": {
    "id": "String",
  },
  "name": "String"
}
```

### <a name="response"></a><span data-ttu-id="4e59f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e59f-143">Response</span></span>

<span data-ttu-id="4e59f-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4e59f-144">The following is an example of the response.</span></span>

> <span data-ttu-id="4e59f-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e59f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1312abc!1231",
  "name": "new-restored-item-name.txt",
  "size": 19121,
  "lastModifiedDateTime": "2017-12-12T10:40:59Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Restore a DriveItem.",
  "keywords": "retore,item,driveitem",
  "section": "documentation",
  "tocPath": "Items/Restore"
}-->