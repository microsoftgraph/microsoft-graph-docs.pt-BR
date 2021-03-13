---
title: Criar marca
description: Crie um novo objeto tag.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 412a0cd1ae4f8c38466a6526a5c84eea670897bb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773757"
---
# <a name="create-tag"></a><span data-ttu-id="0a45b-103">Criar marca</span><span class="sxs-lookup"><span data-stu-id="0a45b-103">Create tag</span></span>

<span data-ttu-id="0a45b-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="0a45b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a45b-105">Crie uma nova marca para o caso especificado.</span><span class="sxs-lookup"><span data-stu-id="0a45b-105">Create a new tag for the specified case.</span></span>  <span data-ttu-id="0a45b-106">As marcas são usadas em conjuntos de revisão durante a revisão do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="0a45b-106">The tags are used in review sets while reviewing content.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a45b-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="0a45b-107">Permissions</span></span>

<span data-ttu-id="0a45b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a45b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a45b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a45b-110">Permission type</span></span>|<span data-ttu-id="0a45b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0a45b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a45b-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a45b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0a45b-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a45b-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="0a45b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a45b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a45b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a45b-115">Not supported.</span></span>|
|<span data-ttu-id="0a45b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a45b-116">Application</span></span>|<span data-ttu-id="0a45b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a45b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a45b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a45b-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/tags
```

## <a name="request-headers"></a><span data-ttu-id="0a45b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a45b-119">Request headers</span></span>

|<span data-ttu-id="0a45b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0a45b-120">Name</span></span>|<span data-ttu-id="0a45b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a45b-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0a45b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a45b-122">Authorization</span></span>|<span data-ttu-id="0a45b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a45b-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0a45b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0a45b-125">Content-Type</span></span>|<span data-ttu-id="0a45b-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a45b-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a45b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a45b-128">Request body</span></span>

<span data-ttu-id="0a45b-129">No corpo da solicitação, fornece uma representação JSON do [objeto tag.](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="0a45b-129">In the request body, supply a JSON representation of the [tag](../resources/ediscovery-tag.md) object.</span></span>

<span data-ttu-id="0a45b-130">A tabela a seguir mostra as propriedades necessárias ao criar a [marca](../resources/ediscovery-tag.md).</span><span class="sxs-lookup"><span data-stu-id="0a45b-130">The following table shows the properties that are required when you create the [tag](../resources/ediscovery-tag.md).</span></span>

|<span data-ttu-id="0a45b-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a45b-131">Property</span></span>|<span data-ttu-id="0a45b-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a45b-132">Type</span></span>|<span data-ttu-id="0a45b-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a45b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a45b-134">childSelectability</span><span class="sxs-lookup"><span data-stu-id="0a45b-134">childSelectability</span></span>|[<span data-ttu-id="0a45b-135">microsoft.graph.ediscovery.childSelectability</span><span class="sxs-lookup"><span data-stu-id="0a45b-135">microsoft.graph.ediscovery.childSelectability</span></span>](../resources/ediscovery-tag.md#childselectability-values)|<span data-ttu-id="0a45b-136">Indica se uma única ou várias marcas filho podem ser associadas a um documento.</span><span class="sxs-lookup"><span data-stu-id="0a45b-136">Indicates whether a single or multiple child tags can be associated with a document.</span></span> <span data-ttu-id="0a45b-137">Os valores possíveis são: `One` e `Many`.</span><span class="sxs-lookup"><span data-stu-id="0a45b-137">Possible values are: `One`, `Many`.</span></span>  <span data-ttu-id="0a45b-138">Esse valor controla se o UX apresenta as marcas como caixas de seleção ou um grupo de botões de rádio.</span><span class="sxs-lookup"><span data-stu-id="0a45b-138">This value controls whether the UX presents the tags as checkboxes or a radio button group.</span></span> <span data-ttu-id="0a45b-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a45b-139">Required.</span></span>|
|<span data-ttu-id="0a45b-140">displayName</span><span class="sxs-lookup"><span data-stu-id="0a45b-140">displayName</span></span>|<span data-ttu-id="0a45b-141">String</span><span class="sxs-lookup"><span data-stu-id="0a45b-141">String</span></span>|<span data-ttu-id="0a45b-142">Nome de exibição da marca.</span><span class="sxs-lookup"><span data-stu-id="0a45b-142">Display name of the tag.</span></span> <span data-ttu-id="0a45b-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a45b-143">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="0a45b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a45b-144">Response</span></span>

<span data-ttu-id="0a45b-145">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a45b-145">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0a45b-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0a45b-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0a45b-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a45b-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0a45b-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a45b-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tag_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags
Content-Type: application/json
Content-length: 235

{
  "displayName":"Privileged",
  "description":"The document is privileged",
  "parent@odata.bind":"https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/98fdad78bbce4519b75474bc150575c3"
}
```
# <a name="c"></a>[<span data-ttu-id="0a45b-149">C#</span><span class="sxs-lookup"><span data-stu-id="0a45b-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tag-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a45b-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a45b-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tag-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a45b-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a45b-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tag-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a45b-152">Java</span><span class="sxs-lookup"><span data-stu-id="0a45b-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tag-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0a45b-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a45b-153">Response</span></span>

<span data-ttu-id="0a45b-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0a45b-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.tag"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/$entity",
    "displayName": "Privileged",
    "description": "The document is privileged",
    "lastModifiedDateTime": "2021-01-12T01:01:09.0419153Z",
    "childSelectability": "One",
    "id": "0825ef81ade74095a3b3154a3c434c3e",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null,
            "userPrincipalName": "admin@contoso.com"
        }
    }
}
```
