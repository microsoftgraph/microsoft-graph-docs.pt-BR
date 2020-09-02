---
title: Atualizar termo
description: Atualiza as propriedades de um objeto Term.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5aebe53a7bec3fffc90bb27c7beb60c89b500942
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330195"
---
# <a name="update-term"></a><span data-ttu-id="22bd8-103">Atualizar termo</span><span class="sxs-lookup"><span data-stu-id="22bd8-103">Update term</span></span>
<span data-ttu-id="22bd8-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="22bd8-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22bd8-105">Atualiza as propriedades de um objeto [Term](../resources/termstore-term.md) .</span><span class="sxs-lookup"><span data-stu-id="22bd8-105">Update the properties of a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="22bd8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="22bd8-106">Permissions</span></span>
<span data-ttu-id="22bd8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22bd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22bd8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22bd8-109">Permission type</span></span>|<span data-ttu-id="22bd8-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22bd8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22bd8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22bd8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="22bd8-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22bd8-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="22bd8-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22bd8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22bd8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22bd8-114">Not supported.</span></span>    |
|<span data-ttu-id="22bd8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22bd8-115">Application</span></span> | <span data-ttu-id="22bd8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22bd8-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="22bd8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22bd8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

``` http
PATCH /termStore/sets/{setId}/terms/{termId}
```

## <a name="request-headers"></a><span data-ttu-id="22bd8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22bd8-118">Request headers</span></span>
|<span data-ttu-id="22bd8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="22bd8-119">Name</span></span>|<span data-ttu-id="22bd8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="22bd8-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="22bd8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="22bd8-121">Authorization</span></span>|<span data-ttu-id="22bd8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22bd8-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="22bd8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="22bd8-124">Content-Type</span></span>|<span data-ttu-id="22bd8-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22bd8-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="22bd8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22bd8-127">Request body</span></span>
<span data-ttu-id="22bd8-128">No corpo da solicitação, forneça uma representação JSON do objeto [Term](../resources/termstore-term.md) .</span><span class="sxs-lookup"><span data-stu-id="22bd8-128">In the request body, supply a JSON representation of the [term](../resources/termstore-term.md) object.</span></span>

<span data-ttu-id="22bd8-129">A tabela a seguir mostra as propriedades que podem ser atualizadas para um [termo](../resources/termstore-term.md).</span><span class="sxs-lookup"><span data-stu-id="22bd8-129">The following table shows the properties that can be updated for a [term](../resources/termstore-term.md).</span></span>

|<span data-ttu-id="22bd8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22bd8-130">Property</span></span>|<span data-ttu-id="22bd8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="22bd8-131">Type</span></span>|<span data-ttu-id="22bd8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="22bd8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22bd8-133">Legendas</span><span class="sxs-lookup"><span data-stu-id="22bd8-133">labels</span></span>|<span data-ttu-id="22bd8-134">coleção [Microsoft. Graph. termos. localizedLabel](../resources/termstore-localizedlabel.md)</span><span class="sxs-lookup"><span data-stu-id="22bd8-134">[microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md) collection</span></span>|<span data-ttu-id="22bd8-135">rótulos de um termo</span><span class="sxs-lookup"><span data-stu-id="22bd8-135">labels of a term</span></span>|
|<span data-ttu-id="22bd8-136">descrições</span><span class="sxs-lookup"><span data-stu-id="22bd8-136">descriptions</span></span>|<span data-ttu-id="22bd8-137">coleção [Microsoft. Graph. termos. localizedDescription](../resources/termstore-localizeddescription.md)</span><span class="sxs-lookup"><span data-stu-id="22bd8-137">[microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md) collection</span></span>|<span data-ttu-id="22bd8-138">descrição sobre o termo</span><span class="sxs-lookup"><span data-stu-id="22bd8-138">description about the term</span></span>|
|<span data-ttu-id="22bd8-139">properties</span><span class="sxs-lookup"><span data-stu-id="22bd8-139">properties</span></span>|<span data-ttu-id="22bd8-140">coleção [Microsoft. Graph. KeyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="22bd8-140">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="22bd8-141">Propriedades associadas ao termo</span><span class="sxs-lookup"><span data-stu-id="22bd8-141">properties associated with the term</span></span>|



## <a name="response"></a><span data-ttu-id="22bd8-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="22bd8-142">Response</span></span>

<span data-ttu-id="22bd8-143">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Term](../resources/termstore-term.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22bd8-143">If successful, this method returns a `200 OK` response code and an updated [term](../resources/termstore-term.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="22bd8-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="22bd8-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="22bd8-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22bd8-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="22bd8-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="22bd8-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_term"
} -->

``` http
PATCH https://graph.microsoft.com/beta/termStore/sets/{setId}/terms/{termId}
Content-Type: application/json
Content-length: 366

{
  "labels" : [
      {
          "name" : "changedLabel",
          "languageTag" : "en-US",
          "isDefault" : true
      }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="22bd8-147">C#</span><span class="sxs-lookup"><span data-stu-id="22bd8-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-term-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22bd8-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22bd8-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-term-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22bd8-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22bd8-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-term-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="22bd8-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="22bd8-150">Response</span></span>
<span data-ttu-id="22bd8-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="22bd8-151">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.term"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "81be9856-9856-81be-5698-be815698be81",
  "labels" : [
      {
          "name" : "changedLabel",
          "languageTag" : "en-US",
          "isDefault" : true
      }
  ]
}
```

[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Get term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Update term",
  "suppressions": [
  ]
}
-->
