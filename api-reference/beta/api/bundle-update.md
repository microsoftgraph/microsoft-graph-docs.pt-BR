---
author: JeremyKelley
ms.author: jeremyke
title: Atualizar um pacote
description: Atualizar um pacote de driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e3d7e684b9987aa5bcd4c601654956c84b6f7904
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944807"
---
# <a name="update-bundle"></a><span data-ttu-id="f70da-103">Pacote de atualização</span><span class="sxs-lookup"><span data-stu-id="f70da-103">Update bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f70da-104">Atualize os metadados de um [pacote][] de [DRIVEITEMS][driveItem] por ID.</span><span class="sxs-lookup"><span data-stu-id="f70da-104">Update the metadata for a [bundle][] of [driveItems][driveItem] by ID.</span></span>
<span data-ttu-id="f70da-105">Você só pode atualizar os seguintes metadados:</span><span class="sxs-lookup"><span data-stu-id="f70da-105">You can only update the following metadata:</span></span>

* <span data-ttu-id="f70da-106">Nome do pacote</span><span class="sxs-lookup"><span data-stu-id="f70da-106">Bundle name</span></span>
* <span data-ttu-id="f70da-107">Álbum `coverImageItemId` (se aplicável)</span><span class="sxs-lookup"><span data-stu-id="f70da-107">Album `coverImageItemId` (if applicable)</span></span>

<span data-ttu-id="f70da-108">Quaisquer outras solicitações de alteração serão ignoradas.</span><span class="sxs-lookup"><span data-stu-id="f70da-108">Any other change requests will be ignored.</span></span>

## <a name="permissions"></a><span data-ttu-id="f70da-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f70da-109">Permissions</span></span>

<span data-ttu-id="f70da-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f70da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f70da-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f70da-112">Permission type</span></span>      | <span data-ttu-id="f70da-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f70da-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f70da-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f70da-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f70da-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f70da-115">Not supported.</span></span>                             |
|<span data-ttu-id="f70da-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f70da-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f70da-117">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f70da-117">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="f70da-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f70da-118">Application</span></span>          | <span data-ttu-id="f70da-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f70da-119">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="f70da-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f70da-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drive/items/{bundle-id}
```

## <a name="request-headers"></a><span data-ttu-id="f70da-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f70da-121">Request headers</span></span>

| <span data-ttu-id="f70da-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f70da-122">Name</span></span>          | <span data-ttu-id="f70da-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f70da-123">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="f70da-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f70da-124">Authorization</span></span> | <span data-ttu-id="f70da-125">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="f70da-125">Bearer \{token\}.</span></span> <span data-ttu-id="f70da-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f70da-126">Required.</span></span> |
| <span data-ttu-id="f70da-127">if-match</span><span class="sxs-lookup"><span data-stu-id="f70da-127">if-match</span></span>      | <span data-ttu-id="f70da-128">ETag.</span><span class="sxs-lookup"><span data-stu-id="f70da-128">eTag.</span></span> <span data-ttu-id="f70da-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f70da-129">Optional.</span></span> <span data-ttu-id="f70da-130">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à eTag atual no buncle, uma `412 Precondition Failed` resposta será retornada.</span><span class="sxs-lookup"><span data-stu-id="f70da-130">If this request header is included and the eTag provided does not match the current eTag on the buncle, a `412 Precondition Failed` response is returned.</span></span>

## <a name="request-body"></a><span data-ttu-id="f70da-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f70da-131">Request body</span></span>

<span data-ttu-id="f70da-132">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="f70da-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f70da-133">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="f70da-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f70da-134">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f70da-134">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="f70da-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f70da-135">Response</span></span>

<span data-ttu-id="f70da-136">Se tiver êxito, este método retornará um recurso [driveItem][] que representa o pacote atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f70da-136">If successful, this method returns a [driveItem][] resource that represents the updated bundle in the response body.</span></span>

<span data-ttu-id="f70da-137">Leia o tópico [respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="f70da-137">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="f70da-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f70da-138">Example</span></span>

<span data-ttu-id="f70da-139">Este exemplo renomeia um pacote.</span><span class="sxs-lookup"><span data-stu-id="f70da-139">This example renames a bundle.</span></span>

### <a name="request"></a><span data-ttu-id="f70da-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f70da-140">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f70da-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="f70da-141">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "rename-bundle" } -->

```json
PATCH https://graph.microsoft.com/beta/drive/items/{bundle-id}
Content-Type: application/json

{
  "name": "Shared legal agreements"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f70da-142">C#</span><span class="sxs-lookup"><span data-stu-id="f70da-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rename-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f70da-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="f70da-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rename-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f70da-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f70da-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rename-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f70da-145">Java</span><span class="sxs-lookup"><span data-stu-id="f70da-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rename-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f70da-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="f70da-146">Response</span></span>

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

<span data-ttu-id="f70da-147">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f70da-147">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f70da-148">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f70da-148">All the properties will be returned from an actual call.</span></span>


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
