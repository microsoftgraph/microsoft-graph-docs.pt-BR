---
author: JeremyKelley
title: Atualizar um pacote
description: Atualizar um pacote de driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5c27690f146924db2ade4baf8539a4973aa01ce2
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471515"
---
# <a name="update-bundle"></a><span data-ttu-id="bc4a4-103">Pacote de atualizações</span><span class="sxs-lookup"><span data-stu-id="bc4a4-103">Update bundle</span></span>

<span data-ttu-id="bc4a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc4a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc4a4-105">Atualize os metadados [para um pacote][] de [driveItems][driveItem] por ID.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-105">Update the metadata for a [bundle][] of [driveItems][driveItem] by ID.</span></span>
<span data-ttu-id="bc4a4-106">Você só pode atualizar os seguintes metadados:</span><span class="sxs-lookup"><span data-stu-id="bc4a4-106">You can only update the following metadata:</span></span>

* <span data-ttu-id="bc4a4-107">Nome do pacote</span><span class="sxs-lookup"><span data-stu-id="bc4a4-107">Bundle name</span></span>
* <span data-ttu-id="bc4a4-108">Album `coverImageItemId` (se aplicável)</span><span class="sxs-lookup"><span data-stu-id="bc4a4-108">Album `coverImageItemId` (if applicable)</span></span>

<span data-ttu-id="bc4a4-109">Quaisquer outras solicitações de alteração serão ignoradas.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-109">Any other change requests will be ignored.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc4a4-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc4a4-110">Permissions</span></span>

<span data-ttu-id="bc4a4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc4a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc4a4-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc4a4-113">Permission type</span></span>      | <span data-ttu-id="bc4a4-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc4a4-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc4a4-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc4a4-115">Delegated (work or school account)</span></span> | <span data-ttu-id="bc4a4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-116">Not supported.</span></span>                             |
|<span data-ttu-id="bc4a4-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc4a4-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc4a4-118">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc4a4-118">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="bc4a4-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc4a4-119">Application</span></span>          | <span data-ttu-id="bc4a4-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-120">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="bc4a4-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc4a4-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drive/items/{bundle-id}
```

## <a name="request-headers"></a><span data-ttu-id="bc4a4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc4a4-122">Request headers</span></span>

| <span data-ttu-id="bc4a4-123">Nome</span><span class="sxs-lookup"><span data-stu-id="bc4a4-123">Name</span></span>          | <span data-ttu-id="bc4a4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc4a4-124">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="bc4a4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc4a4-125">Authorization</span></span> | <span data-ttu-id="bc4a4-126">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-126">Bearer \{token\}.</span></span> <span data-ttu-id="bc4a4-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-127">Required.</span></span> |
| <span data-ttu-id="bc4a4-128">if-match</span><span class="sxs-lookup"><span data-stu-id="bc4a4-128">if-match</span></span>      | <span data-ttu-id="bc4a4-129">eTag.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-129">eTag.</span></span> <span data-ttu-id="bc4a4-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-130">Optional.</span></span> <span data-ttu-id="bc4a4-131">Se esse header de solicitação estiver incluído e a eTag fornecida não corresponder à eTag atual no buncle, uma `412 Precondition Failed` resposta será retornada.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-131">If this request header is included and the eTag provided does not match the current eTag on the buncle, a `412 Precondition Failed` response is returned.</span></span>

## <a name="request-body"></a><span data-ttu-id="bc4a4-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc4a4-132">Request body</span></span>

<span data-ttu-id="bc4a4-133">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bc4a4-134">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bc4a4-135">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-135">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="bc4a4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc4a4-136">Response</span></span>

<span data-ttu-id="bc4a4-137">Se tiver êxito, este método retornará um [recurso driveItem][] que representa o pacote atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-137">If successful, this method returns a [driveItem][] resource that represents the updated bundle in the response body.</span></span>

<span data-ttu-id="bc4a4-138">Leia o tópico [Respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-138">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="bc4a4-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc4a4-139">Example</span></span>

<span data-ttu-id="bc4a4-140">Este exemplo renomeia um pacote.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-140">This example renames a bundle.</span></span>

### <a name="request"></a><span data-ttu-id="bc4a4-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc4a4-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bc4a4-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc4a4-142">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "rename-bundle" } -->

```http
PATCH https://graph.microsoft.com/beta/drive/items/{bundle-id}
Content-Type: application/json

{
  "name": "Shared legal agreements"
}
```
# <a name="c"></a>[<span data-ttu-id="bc4a4-143">C#</span><span class="sxs-lookup"><span data-stu-id="bc4a4-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rename-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc4a4-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc4a4-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rename-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc4a4-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc4a4-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rename-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bc4a4-146">Java</span><span class="sxs-lookup"><span data-stu-id="bc4a4-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rename-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bc4a4-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc4a4-147">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
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

<span data-ttu-id="bc4a4-148">O objeto de resposta mostrado aqui pode ser reduzido para a capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-148">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bc4a4-149">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-149">All the properties will be returned from an actual call.</span></span>


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


