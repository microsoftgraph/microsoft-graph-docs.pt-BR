---
author: JeremyKelley
ms.author: jeremyke
title: Atualizar um pacote
description: Atualizar um pacote de driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 18c04ff7760505901ded5adb6e291fadc7481b35
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441015"
---
# <a name="update-bundle"></a><span data-ttu-id="42111-103">Pacote de atualização</span><span class="sxs-lookup"><span data-stu-id="42111-103">Update bundle</span></span>

<span data-ttu-id="42111-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="42111-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42111-105">Atualize os metadados de um [pacote][] de [DRIVEITEMS][driveItem] por ID.</span><span class="sxs-lookup"><span data-stu-id="42111-105">Update the metadata for a [bundle][] of [driveItems][driveItem] by ID.</span></span>
<span data-ttu-id="42111-106">Você só pode atualizar os seguintes metadados:</span><span class="sxs-lookup"><span data-stu-id="42111-106">You can only update the following metadata:</span></span>

* <span data-ttu-id="42111-107">Nome do pacote</span><span class="sxs-lookup"><span data-stu-id="42111-107">Bundle name</span></span>
* <span data-ttu-id="42111-108">Álbum `coverImageItemId` (se aplicável)</span><span class="sxs-lookup"><span data-stu-id="42111-108">Album `coverImageItemId` (if applicable)</span></span>

<span data-ttu-id="42111-109">Quaisquer outras solicitações de alteração serão ignoradas.</span><span class="sxs-lookup"><span data-stu-id="42111-109">Any other change requests will be ignored.</span></span>

## <a name="permissions"></a><span data-ttu-id="42111-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="42111-110">Permissions</span></span>

<span data-ttu-id="42111-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42111-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42111-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42111-113">Permission type</span></span>      | <span data-ttu-id="42111-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42111-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42111-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42111-115">Delegated (work or school account)</span></span> | <span data-ttu-id="42111-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42111-116">Not supported.</span></span>                             |
|<span data-ttu-id="42111-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42111-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42111-118">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42111-118">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="42111-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42111-119">Application</span></span>          | <span data-ttu-id="42111-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42111-120">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="42111-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42111-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drive/items/{bundle-id}
```

## <a name="request-headers"></a><span data-ttu-id="42111-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42111-122">Request headers</span></span>

| <span data-ttu-id="42111-123">Nome</span><span class="sxs-lookup"><span data-stu-id="42111-123">Name</span></span>          | <span data-ttu-id="42111-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="42111-124">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="42111-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="42111-125">Authorization</span></span> | <span data-ttu-id="42111-126">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="42111-126">Bearer \{token\}.</span></span> <span data-ttu-id="42111-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42111-127">Required.</span></span> |
| <span data-ttu-id="42111-128">if-match</span><span class="sxs-lookup"><span data-stu-id="42111-128">if-match</span></span>      | <span data-ttu-id="42111-129">ETag.</span><span class="sxs-lookup"><span data-stu-id="42111-129">eTag.</span></span> <span data-ttu-id="42111-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="42111-130">Optional.</span></span> <span data-ttu-id="42111-131">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à eTag atual no buncle, uma `412 Precondition Failed` resposta será retornada.</span><span class="sxs-lookup"><span data-stu-id="42111-131">If this request header is included and the eTag provided does not match the current eTag on the buncle, a `412 Precondition Failed` response is returned.</span></span>

## <a name="request-body"></a><span data-ttu-id="42111-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42111-132">Request body</span></span>

<span data-ttu-id="42111-133">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="42111-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="42111-134">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="42111-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="42111-135">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="42111-135">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="42111-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="42111-136">Response</span></span>

<span data-ttu-id="42111-137">Se tiver êxito, este método retornará um recurso [driveItem][] que representa o pacote atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42111-137">If successful, this method returns a [driveItem][] resource that represents the updated bundle in the response body.</span></span>

<span data-ttu-id="42111-138">Leia o tópico [respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="42111-138">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="42111-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42111-139">Example</span></span>

<span data-ttu-id="42111-140">Este exemplo renomeia um pacote.</span><span class="sxs-lookup"><span data-stu-id="42111-140">This example renames a bundle.</span></span>

### <a name="request"></a><span data-ttu-id="42111-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42111-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="42111-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="42111-142">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "rename-bundle" } -->

```json
PATCH https://graph.microsoft.com/beta/drive/items/{bundle-id}
Content-Type: application/json

{
  "name": "Shared legal agreements"
}
```
# <a name="c"></a>[<span data-ttu-id="42111-143">C#</span><span class="sxs-lookup"><span data-stu-id="42111-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rename-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42111-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42111-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rename-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42111-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42111-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rename-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="42111-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="42111-146">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "Shared legal agreements",
  "bundle": {
    "childCount": 3
  }
}
```

<span data-ttu-id="42111-147">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="42111-147">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="42111-148">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42111-148">All the properties will be returned from an actual call.</span></span>


[pacote]: ../resources/bundle.md
[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of a bundle.",
  "keywords": "update,replace,contents,bundle",
  "section": "documentation",
    "tocPath": "Bundles/Update"
} -->
