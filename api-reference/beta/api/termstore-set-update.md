---
title: Conjunto de atualizações
description: Atualizar as propriedades de um objeto set.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: fe2b221bc6e6852af5d8aadcf283e851e1c47872
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872055"
---
# <a name="update-set"></a><span data-ttu-id="1fcb9-103">Conjunto de atualizações</span><span class="sxs-lookup"><span data-stu-id="1fcb9-103">Update set</span></span>
<span data-ttu-id="1fcb9-104">Namespace: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="1fcb9-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fcb9-105">Atualizar as propriedades de um [objeto set.](../resources/termstore-set.md)</span><span class="sxs-lookup"><span data-stu-id="1fcb9-105">Update the properties of a [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fcb9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1fcb9-106">Permissions</span></span>
<span data-ttu-id="1fcb9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fcb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fcb9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fcb9-109">Permission type</span></span>|<span data-ttu-id="1fcb9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1fcb9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fcb9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fcb9-111">Delegated (work or school account)</span></span> |<span data-ttu-id="1fcb9-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fcb9-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="1fcb9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fcb9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fcb9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-114">Not supported.</span></span>    |
|<span data-ttu-id="1fcb9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fcb9-115">Application</span></span> | <span data-ttu-id="1fcb9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="1fcb9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fcb9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /termStore/sets/{setId}
```

## <a name="request-headers"></a><span data-ttu-id="1fcb9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fcb9-118">Request headers</span></span>
|<span data-ttu-id="1fcb9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1fcb9-119">Name</span></span>|<span data-ttu-id="1fcb9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fcb9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1fcb9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fcb9-121">Authorization</span></span>|<span data-ttu-id="1fcb9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1fcb9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1fcb9-124">Content-Type</span></span>|<span data-ttu-id="1fcb9-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fcb9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fcb9-127">Request body</span></span>
<span data-ttu-id="1fcb9-128">No corpo da solicitação, fornece uma representação JSON do [objeto set.](../resources/termstore-set.md)</span><span class="sxs-lookup"><span data-stu-id="1fcb9-128">In the request body, supply a JSON representation of the [set](../resources/termstore-set.md) object.</span></span>

<span data-ttu-id="1fcb9-129">A tabela a seguir mostra as propriedades que podem ser editadas para o [conjunto.](../resources/termstore-set.md)</span><span class="sxs-lookup"><span data-stu-id="1fcb9-129">The following table shows the properties that can be edited for the [set](../resources/termstore-set.md).</span></span>

|<span data-ttu-id="1fcb9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1fcb9-130">Property</span></span>|<span data-ttu-id="1fcb9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fcb9-131">Type</span></span>|<span data-ttu-id="1fcb9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fcb9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fcb9-133">localizedNames</span><span class="sxs-lookup"><span data-stu-id="1fcb9-133">localizedNames</span></span>|<span data-ttu-id="1fcb9-134">[coleção microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md)</span><span class="sxs-lookup"><span data-stu-id="1fcb9-134">[microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md) collection</span></span>|<span data-ttu-id="1fcb9-135">Nome do conjunto</span><span class="sxs-lookup"><span data-stu-id="1fcb9-135">Name of the set</span></span>|
|<span data-ttu-id="1fcb9-136">description</span><span class="sxs-lookup"><span data-stu-id="1fcb9-136">description</span></span>|<span data-ttu-id="1fcb9-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1fcb9-137">String</span></span>|<span data-ttu-id="1fcb9-138">Descrição do conjunto</span><span class="sxs-lookup"><span data-stu-id="1fcb9-138">Description of the set</span></span>|
|<span data-ttu-id="1fcb9-139">properties</span><span class="sxs-lookup"><span data-stu-id="1fcb9-139">properties</span></span>|<span data-ttu-id="1fcb9-140">[coleção microsoft.graph.keyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="1fcb9-140">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="1fcb9-141">de um conjunto</span><span class="sxs-lookup"><span data-stu-id="1fcb9-141">properties of a set</span></span>|



## <a name="response"></a><span data-ttu-id="1fcb9-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fcb9-142">Response</span></span>

<span data-ttu-id="1fcb9-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [set](../resources/termstore-set.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-143">If successful, this method returns a `200 OK` response code and an updated [set](../resources/termstore-set.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1fcb9-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1fcb9-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1fcb9-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fcb9-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1fcb9-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fcb9-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1fcb9-147">C#</span><span class="sxs-lookup"><span data-stu-id="1fcb9-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-set-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1fcb9-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fcb9-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-set-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1fcb9-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fcb9-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-set-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1fcb9-150">Java</span><span class="sxs-lookup"><span data-stu-id="1fcb9-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-set-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1fcb9-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fcb9-151">Response</span></span>

<span data-ttu-id="1fcb9-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1fcb9-152">**Note:** The response object shown here might be shortened for readability.</span></span>

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


