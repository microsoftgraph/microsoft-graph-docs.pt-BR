---
title: Atualizar repositório
description: Atualiza as propriedades de um objeto Store.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: e097cfcb0ae83346433cf9ec9a510174e31a1bc4
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330049"
---
# <a name="update-store"></a><span data-ttu-id="e4a20-103">Atualizar repositório</span><span class="sxs-lookup"><span data-stu-id="e4a20-103">Update store</span></span>
<span data-ttu-id="e4a20-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="e4a20-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4a20-105">Atualiza as propriedades de um objeto [Store](../resources/termstore-store.md) .</span><span class="sxs-lookup"><span data-stu-id="e4a20-105">Update the properties of a [store](../resources/termstore-store.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4a20-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4a20-106">Permissions</span></span>
<span data-ttu-id="e4a20-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4a20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4a20-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4a20-109">Permission type</span></span>|<span data-ttu-id="e4a20-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e4a20-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4a20-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4a20-111">Delegated (work or school account)</span></span> |<span data-ttu-id="e4a20-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4a20-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="e4a20-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4a20-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4a20-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4a20-114">Not supported.</span></span>    |
|<span data-ttu-id="e4a20-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4a20-115">Application</span></span> | <span data-ttu-id="e4a20-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4a20-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4a20-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4a20-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

``` http
PATCH /termStore
```

## <a name="request-headers"></a><span data-ttu-id="e4a20-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4a20-118">Request headers</span></span>
|<span data-ttu-id="e4a20-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e4a20-119">Name</span></span>|<span data-ttu-id="e4a20-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4a20-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e4a20-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4a20-121">Authorization</span></span>|<span data-ttu-id="e4a20-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4a20-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e4a20-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e4a20-124">Content-Type</span></span>|<span data-ttu-id="e4a20-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4a20-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4a20-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4a20-127">Request body</span></span>
<span data-ttu-id="e4a20-128">No corpo da solicitação, forneça uma representação JSON do objeto [Store](../resources/termstore-store.md) .</span><span class="sxs-lookup"><span data-stu-id="e4a20-128">In the request body, supply a JSON representation of the [store](../resources/termstore-store.md) object.</span></span>

<span data-ttu-id="e4a20-129">A tabela a seguir mostra as propriedades que podem ser editadas para o [repositório](../resources/termstore-store.md).</span><span class="sxs-lookup"><span data-stu-id="e4a20-129">The following table shows the properties that can be edited for the [store](../resources/termstore-store.md).</span></span>

|<span data-ttu-id="e4a20-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4a20-130">Property</span></span>|<span data-ttu-id="e4a20-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4a20-131">Type</span></span>|<span data-ttu-id="e4a20-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4a20-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4a20-133">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="e4a20-133">defaultLanguageTag</span></span>|<span data-ttu-id="e4a20-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4a20-134">String</span></span>|<span data-ttu-id="e4a20-135">Idioma padrão do [Microsoft. Graph. termos. Store](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="e4a20-135">Default language of the [microsoft.graph.termstore.store](../resources/termstore-store.md)</span></span>|
|<span data-ttu-id="e4a20-136">languageTags</span><span class="sxs-lookup"><span data-stu-id="e4a20-136">languageTags</span></span>|<span data-ttu-id="e4a20-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4a20-137">String collection</span></span>|<span data-ttu-id="e4a20-138">Idiomas disponíveis no [Microsoft. Graph. termos. Store](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="e4a20-138">Available languages in the [microsoft.graph.termstore.store](../resources/termstore-store.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e4a20-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4a20-139">Response</span></span>

<span data-ttu-id="e4a20-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Store](../resources/termstore-store.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4a20-140">If successful, this method returns a `200 OK` response code and an updated [store](../resources/termstore-store.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e4a20-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e4a20-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e4a20-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4a20-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e4a20-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4a20-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_store"
} -->

``` http
PATCH https://graph.microsoft.com/beta/termStore
Content-Type: application/json
Content-length: 133

{
  "defaultLanguageTag": "en-US"
}
```
# <a name="javascript"></a>[<span data-ttu-id="e4a20-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4a20-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4a20-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4a20-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="e4a20-146">C#</span><span class="sxs-lookup"><span data-stu-id="e4a20-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-store-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e4a20-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4a20-147">Response</span></span>
<span data-ttu-id="e4a20-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e4a20-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.store"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "dad13b4b-3b4b-dad1-4b3b-d1da4b3bd1da",
  "defaultLanguageTag": "en-US",
  "languageTags": [
    "en-US", 
    "fr-FR"
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Update termstore",
  "suppressions": [
  ]
}
-->

