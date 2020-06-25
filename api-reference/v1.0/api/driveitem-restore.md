---
title: 'driveItem: restaurar'
description: Restaurar um driveItem que foi excluído e que está atualmente na lixeira.
localization_priority: Normal
author: learafa
ms.prod: files
doc_type: apiPageType
ms.openlocfilehash: 152cfaa235fb11c23c656d82da63f839319f2950
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863793"
---
# <a name="driveitem-restore"></a><span data-ttu-id="92cf3-103">driveItem: restaurar</span><span class="sxs-lookup"><span data-stu-id="92cf3-103">driveItem: restore</span></span>

<span data-ttu-id="92cf3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92cf3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="92cf3-105">Restaurar um [driveItem](../resources/driveitem.md) que foi excluído e que está atualmente na lixeira.</span><span class="sxs-lookup"><span data-stu-id="92cf3-105">Restore a [driveItem](../resources/driveitem.md) that has been deleted and is currently in the recycle bin.</span></span> <span data-ttu-id="92cf3-106">**Observação**: atualmente, essa funcionalidade só está disponível para o onedrive Personal.</span><span class="sxs-lookup"><span data-stu-id="92cf3-106">**NOTE**: This functionality is currently only available for OneDrive Personal.</span></span>

## <a name="permissions"></a><span data-ttu-id="92cf3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="92cf3-107">Permissions</span></span>

<span data-ttu-id="92cf3-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="92cf3-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="92cf3-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92cf3-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="92cf3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92cf3-110">Permission type</span></span>                        | <span data-ttu-id="92cf3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92cf3-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="92cf3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92cf3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="92cf3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92cf3-113">Not supported.</span></span> |
| <span data-ttu-id="92cf3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92cf3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92cf3-115">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92cf3-115">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="92cf3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92cf3-116">Application</span></span>                            | <span data-ttu-id="92cf3-117">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92cf3-117">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="92cf3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92cf3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/drive/items/{item-id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="92cf3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92cf3-119">Request headers</span></span>

| <span data-ttu-id="92cf3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="92cf3-120">Name</span></span>          | <span data-ttu-id="92cf3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="92cf3-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="92cf3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="92cf3-122">Authorization</span></span> | <span data-ttu-id="92cf3-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="92cf3-123">Bearer {token}.</span></span> <span data-ttu-id="92cf3-124">Required.</span><span class="sxs-lookup"><span data-stu-id="92cf3-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92cf3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92cf3-125">Request body</span></span>

<span data-ttu-id="92cf3-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92cf3-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="92cf3-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="92cf3-127">Parameter</span></span>     | <span data-ttu-id="92cf3-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="92cf3-128">Type</span></span>                                         | <span data-ttu-id="92cf3-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="92cf3-129">Description</span></span> |
|:--------------|:---------------------------------------------|:------------|
|<span data-ttu-id="92cf3-130">parentReference</span><span class="sxs-lookup"><span data-stu-id="92cf3-130">parentReference</span></span>|[<span data-ttu-id="92cf3-131">ItemReference</span><span class="sxs-lookup"><span data-stu-id="92cf3-131">ItemReference</span></span>](../resources/itemreference.md)| <span data-ttu-id="92cf3-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="92cf3-132">Optional.</span></span> <span data-ttu-id="92cf3-133">Referência ao item pai no qual o item excluído será restaurado.</span><span class="sxs-lookup"><span data-stu-id="92cf3-133">Reference to the parent item the deleted item will be restored to.</span></span> |
|<span data-ttu-id="92cf3-134">nome</span><span class="sxs-lookup"><span data-stu-id="92cf3-134">name</span></span>           |<span data-ttu-id="92cf3-135">String</span><span class="sxs-lookup"><span data-stu-id="92cf3-135">String</span></span>                                        | <span data-ttu-id="92cf3-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="92cf3-136">Optional.</span></span> <span data-ttu-id="92cf3-137">O novo nome do item restaurado.</span><span class="sxs-lookup"><span data-stu-id="92cf3-137">The new name for the restored item.</span></span> <span data-ttu-id="92cf3-138">Se isso não for fornecido, será usado o mesmo nome que o original.</span><span class="sxs-lookup"><span data-stu-id="92cf3-138">If this isn't provided, the same name will be used as the original.</span></span> |

## <a name="response"></a><span data-ttu-id="92cf3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="92cf3-139">Response</span></span>

<span data-ttu-id="92cf3-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [driveItem](../resources/driveitem.md) restaurado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92cf3-140">If successful, this method returns a `200 OK` response code and the restored [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="92cf3-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="92cf3-141">Examples</span></span>

<span data-ttu-id="92cf3-142">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="92cf3-142">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="92cf3-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92cf3-143">Request</span></span>

<span data-ttu-id="92cf3-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="92cf3-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="92cf3-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="92cf3-145">HTTP</span></span>](#tab/http)
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

### <a name="response"></a><span data-ttu-id="92cf3-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="92cf3-146">Response</span></span>

<span data-ttu-id="92cf3-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="92cf3-147">The following is an example of the response.</span></span>

> <span data-ttu-id="92cf3-148">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="92cf3-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="92cf3-149">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="92cf3-149">All the properties will be returned from an actual call.</span></span>

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
