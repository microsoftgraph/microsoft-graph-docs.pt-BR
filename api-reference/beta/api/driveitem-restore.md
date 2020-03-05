---
title: 'driveItem: restaurar'
description: Restaurar um driveItem que foi excluído e que está atualmente na lixeira.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
ms.date: 08/06/2019
doc_type: apiPageType
ms.openlocfilehash: b2dbdca5ff9ab0c55a721b0d47db174ed00bf8c5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432408"
---
# <a name="driveitem-restore"></a><span data-ttu-id="e2155-103">driveItem: restaurar</span><span class="sxs-lookup"><span data-stu-id="e2155-103">driveItem: restore</span></span>

<span data-ttu-id="e2155-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e2155-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2155-105">Restaurar um [driveItem](../resources/driveitem.md) que foi excluído e que está atualmente na lixeira.</span><span class="sxs-lookup"><span data-stu-id="e2155-105">Restore a [driveItem](../resources/driveitem.md) that has been deleted and is currently in the recycle bin.</span></span> <span data-ttu-id="e2155-106">**Observação**: atualmente, essa funcionalidade só está disponível para o onedrive Personal.</span><span class="sxs-lookup"><span data-stu-id="e2155-106">**NOTE**: This functionality is currently only available for OneDrive Personal.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2155-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e2155-107">Permissions</span></span>

<span data-ttu-id="e2155-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2155-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e2155-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2155-110">Permission type</span></span>                        | <span data-ttu-id="e2155-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2155-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e2155-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2155-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e2155-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2155-113">Not supported.</span></span> |
| <span data-ttu-id="e2155-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2155-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2155-115">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2155-115">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="e2155-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2155-116">Application</span></span>                            | <span data-ttu-id="e2155-117">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2155-117">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2155-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2155-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/drive/items/{item-id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="e2155-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2155-119">Request headers</span></span>

| <span data-ttu-id="e2155-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e2155-120">Name</span></span>          | <span data-ttu-id="e2155-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2155-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e2155-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2155-122">Authorization</span></span> | <span data-ttu-id="e2155-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="e2155-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2155-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2155-124">Request body</span></span>

<span data-ttu-id="e2155-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2155-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e2155-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e2155-126">Parameter</span></span>     | <span data-ttu-id="e2155-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2155-127">Type</span></span>                                         | <span data-ttu-id="e2155-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2155-128">Description</span></span> |
|:--------------|:---------------------------------------------|:------------|
|<span data-ttu-id="e2155-129">parentReference</span><span class="sxs-lookup"><span data-stu-id="e2155-129">parentReference</span></span>|[<span data-ttu-id="e2155-130">ItemReference</span><span class="sxs-lookup"><span data-stu-id="e2155-130">ItemReference</span></span>](../resources/itemreference.md)| <span data-ttu-id="e2155-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e2155-131">Optional.</span></span> <span data-ttu-id="e2155-132">Referência ao item pai no qual o item excluído será restaurado.</span><span class="sxs-lookup"><span data-stu-id="e2155-132">Reference to the parent item the deleted item will be restored to.</span></span> |
|<span data-ttu-id="e2155-133">nome</span><span class="sxs-lookup"><span data-stu-id="e2155-133">name</span></span>           |<span data-ttu-id="e2155-134">String</span><span class="sxs-lookup"><span data-stu-id="e2155-134">String</span></span>                                        | <span data-ttu-id="e2155-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e2155-135">Optional.</span></span> <span data-ttu-id="e2155-136">O novo nome do item restaurado.</span><span class="sxs-lookup"><span data-stu-id="e2155-136">The new name for the restored item.</span></span> <span data-ttu-id="e2155-137">Se isso não for fornecido, será usado o mesmo nome que o original.</span><span class="sxs-lookup"><span data-stu-id="e2155-137">If this isn't provided, the same name will be used as the original.</span></span> |

## <a name="response"></a><span data-ttu-id="e2155-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2155-138">Response</span></span>

<span data-ttu-id="e2155-139">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [driveItem](../resources/driveitem.md) restaurado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2155-139">If successful, this method returns `200 OK` response code and the restored [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e2155-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e2155-140">Examples</span></span>

<span data-ttu-id="e2155-141">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e2155-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="e2155-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2155-142">Request</span></span>

<span data-ttu-id="e2155-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2155-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e2155-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2155-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e2155-145">C#</span><span class="sxs-lookup"><span data-stu-id="e2155-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2155-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2155-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2155-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2155-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e2155-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2155-148">Response</span></span>

<span data-ttu-id="e2155-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e2155-149">The following is an example of the response.</span></span>

> <span data-ttu-id="e2155-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2155-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
