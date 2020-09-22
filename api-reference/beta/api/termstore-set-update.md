---
title: Conjunto de atualização
description: Atualiza as propriedades de um objeto Set.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 3ace6599bab823911dcd5704b7424e198daa4e30
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064581"
---
# <a name="update-set"></a><span data-ttu-id="4052a-103">Conjunto de atualização</span><span class="sxs-lookup"><span data-stu-id="4052a-103">Update set</span></span>
<span data-ttu-id="4052a-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="4052a-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4052a-105">Atualiza as propriedades de um objeto [set](../resources/termstore-set.md) .</span><span class="sxs-lookup"><span data-stu-id="4052a-105">Update the properties of a [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4052a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4052a-106">Permissions</span></span>
<span data-ttu-id="4052a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4052a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4052a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4052a-109">Permission type</span></span>|<span data-ttu-id="4052a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4052a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4052a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4052a-111">Delegated (work or school account)</span></span> |<span data-ttu-id="4052a-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4052a-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="4052a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4052a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4052a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4052a-114">Not supported.</span></span>    |
|<span data-ttu-id="4052a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4052a-115">Application</span></span> | <span data-ttu-id="4052a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4052a-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="4052a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4052a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /termStore/sets/{setId}
```

## <a name="request-headers"></a><span data-ttu-id="4052a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4052a-118">Request headers</span></span>
|<span data-ttu-id="4052a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4052a-119">Name</span></span>|<span data-ttu-id="4052a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4052a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4052a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4052a-121">Authorization</span></span>|<span data-ttu-id="4052a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4052a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4052a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4052a-124">Content-Type</span></span>|<span data-ttu-id="4052a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4052a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4052a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4052a-127">Request body</span></span>
<span data-ttu-id="4052a-128">No corpo da solicitação, forneça uma representação JSON do objeto [set](../resources/termstore-set.md) .</span><span class="sxs-lookup"><span data-stu-id="4052a-128">In the request body, supply a JSON representation of the [set](../resources/termstore-set.md) object.</span></span>

<span data-ttu-id="4052a-129">A tabela a seguir mostra as propriedades que podem ser editadas para o [conjunto](../resources/termstore-set.md).</span><span class="sxs-lookup"><span data-stu-id="4052a-129">The following table shows the properties that can be edited for the [set](../resources/termstore-set.md).</span></span>

|<span data-ttu-id="4052a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4052a-130">Property</span></span>|<span data-ttu-id="4052a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4052a-131">Type</span></span>|<span data-ttu-id="4052a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4052a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4052a-133">localizadores</span><span class="sxs-lookup"><span data-stu-id="4052a-133">localizedNames</span></span>|<span data-ttu-id="4052a-134">coleção [Microsoft. Graph. termos.](../resources/termstore-localizedname.md) undeleble</span><span class="sxs-lookup"><span data-stu-id="4052a-134">[microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md) collection</span></span>|<span data-ttu-id="4052a-135">Nome do conjunto</span><span class="sxs-lookup"><span data-stu-id="4052a-135">Name of the set</span></span>|
|<span data-ttu-id="4052a-136">description</span><span class="sxs-lookup"><span data-stu-id="4052a-136">description</span></span>|<span data-ttu-id="4052a-137">String</span><span class="sxs-lookup"><span data-stu-id="4052a-137">String</span></span>|<span data-ttu-id="4052a-138">Descrição do conjunto</span><span class="sxs-lookup"><span data-stu-id="4052a-138">Description of the set</span></span>|
|<span data-ttu-id="4052a-139">properties</span><span class="sxs-lookup"><span data-stu-id="4052a-139">properties</span></span>|<span data-ttu-id="4052a-140">coleção [Microsoft. Graph. KeyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="4052a-140">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="4052a-141">Propriedades de um conjunto</span><span class="sxs-lookup"><span data-stu-id="4052a-141">properties of a set</span></span>|



## <a name="response"></a><span data-ttu-id="4052a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="4052a-142">Response</span></span>

<span data-ttu-id="4052a-143">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [set](../resources/termstore-set.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4052a-143">If successful, this method returns a `200 OK` response code and an updated [set](../resources/termstore-set.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4052a-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4052a-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4052a-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4052a-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4052a-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="4052a-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4052a-147">C#</span><span class="sxs-lookup"><span data-stu-id="4052a-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-set-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4052a-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4052a-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-set-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4052a-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4052a-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-set-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4052a-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="4052a-150">Response</span></span>

<span data-ttu-id="4052a-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4052a-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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


