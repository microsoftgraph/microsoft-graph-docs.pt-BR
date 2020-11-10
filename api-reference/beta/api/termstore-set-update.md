---
title: Conjunto de atualização
description: Atualiza as propriedades de um objeto Set.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 735d565e6929a2b66437b8621d4ab2629e1761ad
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972372"
---
# <a name="update-set"></a><span data-ttu-id="b9fc1-103">Conjunto de atualização</span><span class="sxs-lookup"><span data-stu-id="b9fc1-103">Update set</span></span>
<span data-ttu-id="b9fc1-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="b9fc1-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9fc1-105">Atualiza as propriedades de um objeto [set](../resources/termstore-set.md) .</span><span class="sxs-lookup"><span data-stu-id="b9fc1-105">Update the properties of a [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9fc1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b9fc1-106">Permissions</span></span>
<span data-ttu-id="b9fc1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9fc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9fc1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9fc1-109">Permission type</span></span>|<span data-ttu-id="b9fc1-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b9fc1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9fc1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9fc1-111">Delegated (work or school account)</span></span> |<span data-ttu-id="b9fc1-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9fc1-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="b9fc1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9fc1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9fc1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9fc1-114">Not supported.</span></span>    |
|<span data-ttu-id="b9fc1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9fc1-115">Application</span></span> | <span data-ttu-id="b9fc1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9fc1-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="b9fc1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9fc1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /termStore/sets/{setId}
```

## <a name="request-headers"></a><span data-ttu-id="b9fc1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9fc1-118">Request headers</span></span>
|<span data-ttu-id="b9fc1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b9fc1-119">Name</span></span>|<span data-ttu-id="b9fc1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9fc1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b9fc1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9fc1-121">Authorization</span></span>|<span data-ttu-id="b9fc1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9fc1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b9fc1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b9fc1-124">Content-Type</span></span>|<span data-ttu-id="b9fc1-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9fc1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9fc1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9fc1-127">Request body</span></span>
<span data-ttu-id="b9fc1-128">No corpo da solicitação, forneça uma representação JSON do objeto [set](../resources/termstore-set.md) .</span><span class="sxs-lookup"><span data-stu-id="b9fc1-128">In the request body, supply a JSON representation of the [set](../resources/termstore-set.md) object.</span></span>

<span data-ttu-id="b9fc1-129">A tabela a seguir mostra as propriedades que podem ser editadas para o [conjunto](../resources/termstore-set.md).</span><span class="sxs-lookup"><span data-stu-id="b9fc1-129">The following table shows the properties that can be edited for the [set](../resources/termstore-set.md).</span></span>

|<span data-ttu-id="b9fc1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9fc1-130">Property</span></span>|<span data-ttu-id="b9fc1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9fc1-131">Type</span></span>|<span data-ttu-id="b9fc1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9fc1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9fc1-133">localizadores</span><span class="sxs-lookup"><span data-stu-id="b9fc1-133">localizedNames</span></span>|<span data-ttu-id="b9fc1-134">coleção [Microsoft. Graph. termos.](../resources/termstore-localizedname.md) undeleble</span><span class="sxs-lookup"><span data-stu-id="b9fc1-134">[microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md) collection</span></span>|<span data-ttu-id="b9fc1-135">Nome do conjunto</span><span class="sxs-lookup"><span data-stu-id="b9fc1-135">Name of the set</span></span>|
|<span data-ttu-id="b9fc1-136">description</span><span class="sxs-lookup"><span data-stu-id="b9fc1-136">description</span></span>|<span data-ttu-id="b9fc1-137">String</span><span class="sxs-lookup"><span data-stu-id="b9fc1-137">String</span></span>|<span data-ttu-id="b9fc1-138">Descrição do conjunto</span><span class="sxs-lookup"><span data-stu-id="b9fc1-138">Description of the set</span></span>|
|<span data-ttu-id="b9fc1-139">properties</span><span class="sxs-lookup"><span data-stu-id="b9fc1-139">properties</span></span>|<span data-ttu-id="b9fc1-140">coleção [Microsoft. Graph. KeyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b9fc1-140">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="b9fc1-141">Propriedades de um conjunto</span><span class="sxs-lookup"><span data-stu-id="b9fc1-141">properties of a set</span></span>|



## <a name="response"></a><span data-ttu-id="b9fc1-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9fc1-142">Response</span></span>

<span data-ttu-id="b9fc1-143">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [set](../resources/termstore-set.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9fc1-143">If successful, this method returns a `200 OK` response code and an updated [set](../resources/termstore-set.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9fc1-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b9fc1-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b9fc1-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9fc1-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b9fc1-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9fc1-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_set"
} -->

``` http
PATCH https://graph.microsoft.com/beta/termStore/sets/{setId}
Content-Type: application/json
Content-length: 288

{
  "description": "mySet"
}
```
# <a name="c"></a>[<span data-ttu-id="b9fc1-147">C#</span><span class="sxs-lookup"><span data-stu-id="b9fc1-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-set-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9fc1-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9fc1-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-set-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9fc1-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9fc1-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-set-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9fc1-150">Java</span><span class="sxs-lookup"><span data-stu-id="b9fc1-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-set-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b9fc1-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9fc1-151">Response</span></span>

<span data-ttu-id="b9fc1-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b9fc1-152">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.set"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "3607e9f9-e9f9-3607-f9e9-0736f9e90736",
  "description": "mySet",    
  "localizedNames" : [
    {
      "languageTag" : "en-US",
      "name" : "Department"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Update termSet",
  "suppressions": [
  ]
}
-->


