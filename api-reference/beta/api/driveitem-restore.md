---
title: 'driveItem: restaurar'
description: Restaurar um driveItem que foi excluído e que está atualmente na lixeira.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
ms.date: 08/06/2019
doc_type: apiPageType
ms.openlocfilehash: f105ab748e6fff69f1138e4318ac66597a721391
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356293"
---
# <a name="driveitem-restore"></a><span data-ttu-id="05c90-103">driveItem: restaurar</span><span class="sxs-lookup"><span data-stu-id="05c90-103">driveItem: restore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05c90-104">Restaurar um [driveItem](../resources/driveitem.md) que foi excluído e que está atualmente na lixeira.</span><span class="sxs-lookup"><span data-stu-id="05c90-104">Restore a [driveItem](../resources/driveitem.md) that has been deleted and is currently in the recycle bin.</span></span> <span data-ttu-id="05c90-105">**Observação**: atualmente, essa funcionalidade só está disponível para o onedrive Personal.</span><span class="sxs-lookup"><span data-stu-id="05c90-105">**NOTE**: This functionality is currently only available for OneDrive Personal.</span></span>

## <a name="permissions"></a><span data-ttu-id="05c90-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="05c90-106">Permissions</span></span>

<span data-ttu-id="05c90-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05c90-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="05c90-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05c90-109">Permission type</span></span>                        | <span data-ttu-id="05c90-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05c90-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="05c90-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05c90-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="05c90-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05c90-112">Not supported.</span></span> |
| <span data-ttu-id="05c90-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05c90-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05c90-114">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05c90-114">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="05c90-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05c90-115">Application</span></span>                            | <span data-ttu-id="05c90-116">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05c90-116">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05c90-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05c90-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/drive/items/{item-id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="05c90-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05c90-118">Request headers</span></span>

| <span data-ttu-id="05c90-119">Nome</span><span class="sxs-lookup"><span data-stu-id="05c90-119">Name</span></span>          | <span data-ttu-id="05c90-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="05c90-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="05c90-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="05c90-121">Authorization</span></span> | <span data-ttu-id="05c90-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="05c90-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="05c90-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05c90-123">Request body</span></span>

<span data-ttu-id="05c90-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05c90-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="05c90-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="05c90-125">Parameter</span></span>     | <span data-ttu-id="05c90-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="05c90-126">Type</span></span>                                         | <span data-ttu-id="05c90-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="05c90-127">Description</span></span> |
|:--------------|:---------------------------------------------|:------------|
|<span data-ttu-id="05c90-128">parentReference</span><span class="sxs-lookup"><span data-stu-id="05c90-128">parentReference</span></span>|[<span data-ttu-id="05c90-129">ItemReference</span><span class="sxs-lookup"><span data-stu-id="05c90-129">ItemReference</span></span>](../resources/itemreference.md)| <span data-ttu-id="05c90-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="05c90-130">Optional.</span></span> <span data-ttu-id="05c90-131">Referência ao item pai no qual o item excluído será restaurado.</span><span class="sxs-lookup"><span data-stu-id="05c90-131">Reference to the parent item the deleted item will be restored to.</span></span> |
|<span data-ttu-id="05c90-132">name</span><span class="sxs-lookup"><span data-stu-id="05c90-132">name</span></span>           |<span data-ttu-id="05c90-133">String</span><span class="sxs-lookup"><span data-stu-id="05c90-133">String</span></span>                                        | <span data-ttu-id="05c90-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="05c90-134">Optional.</span></span> <span data-ttu-id="05c90-135">O novo nome do item restaurado.</span><span class="sxs-lookup"><span data-stu-id="05c90-135">The new name for the restored item.</span></span> <span data-ttu-id="05c90-136">Se isso não for fornecido, será usado o mesmo nome que o original.</span><span class="sxs-lookup"><span data-stu-id="05c90-136">If this isn't provided, the same name will be used as the original.</span></span> |

## <a name="response"></a><span data-ttu-id="05c90-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="05c90-137">Response</span></span>

<span data-ttu-id="05c90-138">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [driveItem](../resources/driveitem.md) restaurado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05c90-138">If successful, this method returns `200 OK` response code and the restored [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="05c90-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="05c90-139">Examples</span></span>

<span data-ttu-id="05c90-140">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="05c90-140">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="05c90-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05c90-141">Request</span></span>

<span data-ttu-id="05c90-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="05c90-142">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="05c90-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="05c90-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="05c90-144">C#</span><span class="sxs-lookup"><span data-stu-id="05c90-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="05c90-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05c90-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="05c90-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05c90-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="05c90-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="05c90-147">Response</span></span>

<span data-ttu-id="05c90-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="05c90-148">The following is an example of the response.</span></span>

> <span data-ttu-id="05c90-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05c90-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
