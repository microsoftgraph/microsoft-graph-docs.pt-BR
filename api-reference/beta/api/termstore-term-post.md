---
title: Criar termo
description: Criar um novo objeto Term.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8833dea03f14e0b91b6f7e008d16b52aed4f3898
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042830"
---
# <a name="create-term"></a><span data-ttu-id="de5d4-103">Criar termo</span><span class="sxs-lookup"><span data-stu-id="de5d4-103">Create term</span></span>
<span data-ttu-id="de5d4-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="de5d4-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de5d4-105">Criar um novo objeto [Term](../resources/termstore-term.md) .</span><span class="sxs-lookup"><span data-stu-id="de5d4-105">Create a new [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="de5d4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="de5d4-106">Permissions</span></span>
<span data-ttu-id="de5d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de5d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de5d4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de5d4-109">Permission type</span></span>|<span data-ttu-id="de5d4-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="de5d4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de5d4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de5d4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="de5d4-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de5d4-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="de5d4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de5d4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de5d4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de5d4-114">Not supported.</span></span>    |
|<span data-ttu-id="de5d4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de5d4-115">Application</span></span> | <span data-ttu-id="de5d4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de5d4-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="de5d4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de5d4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
} -->

``` http
POST /termStore/sets/{setId}/children
POST /termStore/sets/{setId}/terms/{termId}/children
```

## <a name="request-headers"></a><span data-ttu-id="de5d4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de5d4-118">Request headers</span></span>
|<span data-ttu-id="de5d4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="de5d4-119">Name</span></span>|<span data-ttu-id="de5d4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="de5d4-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="de5d4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="de5d4-121">Authorization</span></span>|<span data-ttu-id="de5d4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de5d4-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="de5d4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="de5d4-124">Content-Type</span></span>|<span data-ttu-id="de5d4-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de5d4-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="de5d4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de5d4-127">Request body</span></span>
<span data-ttu-id="de5d4-128">No corpo da solicitação, forneça uma representação JSON do objeto [Term](../resources/termstore-term.md) .</span><span class="sxs-lookup"><span data-stu-id="de5d4-128">In the request body, supply a JSON representation of the [term](../resources/termstore-term.md) object.</span></span>

<span data-ttu-id="de5d4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o [termo](../resources/termstore-term.md).</span><span class="sxs-lookup"><span data-stu-id="de5d4-129">The following table shows the properties that are required when you create the [term](../resources/termstore-term.md).</span></span>

|<span data-ttu-id="de5d4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de5d4-130">Property</span></span>|<span data-ttu-id="de5d4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="de5d4-131">Type</span></span>|<span data-ttu-id="de5d4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="de5d4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de5d4-133">Legendas</span><span class="sxs-lookup"><span data-stu-id="de5d4-133">labels</span></span>|<span data-ttu-id="de5d4-134">coleção [Microsoft. Graph. termos. localizedLabel](../resources/termstore-localizedlabel.md)</span><span class="sxs-lookup"><span data-stu-id="de5d4-134">[microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md) collection</span></span>|<span data-ttu-id="de5d4-135">Rótulo do termo a ser criado</span><span class="sxs-lookup"><span data-stu-id="de5d4-135">Label for the term to be created</span></span>|



## <a name="response"></a><span data-ttu-id="de5d4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="de5d4-136">Response</span></span>

<span data-ttu-id="de5d4-137">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [Term](../resources/termstore-term.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de5d4-137">If successful, this method returns a `201 Created` response code and a [term](../resources/termstore-term.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="de5d4-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="de5d4-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="de5d4-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de5d4-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="de5d4-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="de5d4-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_term_from_"
} -->

``` http
POST https://graph.microsoft.com/beta/termStore/sets/{setId}/terms
Content-Type: application/json
Content-length: 366

{
  "labels": [
    {
      "languageTag" : "en-US",
      "name" : "Car",
      "isDefault" : true
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="de5d4-141">C#</span><span class="sxs-lookup"><span data-stu-id="de5d4-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-term-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de5d4-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de5d4-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-term-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de5d4-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de5d4-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-term-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="de5d4-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="de5d4-144">Response</span></span>
<span data-ttu-id="de5d4-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="de5d4-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.term"
}-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "createdDateTime": "2019-06-21T20:01:37Z",
  "id": "8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f",
  "labels" : [
      {
          "name" : "Car",
          "languageTag" : "en-US",
          "isDefault" : true
      }
  ],
  "lastModifiedDateTime": "2019-06-21T20:01:37Z"
}
```

[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Post term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Post term",
  "suppressions": [
  ]
}
-->


