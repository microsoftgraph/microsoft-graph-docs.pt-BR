---
title: Atualizar loja
description: Atualizar as propriedades de um objeto store.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 73d1fb22b92c134fc4ebb2b15fe4b9314dce2d5d
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874099"
---
# <a name="update-store"></a><span data-ttu-id="6e354-103">Atualizar loja</span><span class="sxs-lookup"><span data-stu-id="6e354-103">Update store</span></span>
<span data-ttu-id="6e354-104">Namespace: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="6e354-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e354-105">Atualizar as propriedades de um [objeto store.](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="6e354-105">Update the properties of a [store](../resources/termstore-store.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e354-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6e354-106">Permissions</span></span>
<span data-ttu-id="6e354-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e354-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e354-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e354-109">Permission type</span></span>|<span data-ttu-id="6e354-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6e354-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e354-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e354-111">Delegated (work or school account)</span></span> |<span data-ttu-id="6e354-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e354-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="6e354-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e354-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e354-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e354-114">Not supported.</span></span>    |
|<span data-ttu-id="6e354-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e354-115">Application</span></span> | <span data-ttu-id="6e354-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e354-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e354-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e354-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

``` http
PATCH /termStore
```

## <a name="request-headers"></a><span data-ttu-id="6e354-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e354-118">Request headers</span></span>
|<span data-ttu-id="6e354-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6e354-119">Name</span></span>|<span data-ttu-id="6e354-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e354-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6e354-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e354-121">Authorization</span></span>|<span data-ttu-id="6e354-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e354-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6e354-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e354-124">Content-Type</span></span>|<span data-ttu-id="6e354-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e354-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e354-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e354-127">Request body</span></span>
<span data-ttu-id="6e354-128">No corpo da solicitação, fornece uma representação JSON do [objeto store.](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="6e354-128">In the request body, supply a JSON representation of the [store](../resources/termstore-store.md) object.</span></span>

<span data-ttu-id="6e354-129">A tabela a seguir mostra as propriedades que podem ser editadas para o [armazenamento.](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="6e354-129">The following table shows the properties that can be edited for the [store](../resources/termstore-store.md).</span></span>

|<span data-ttu-id="6e354-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e354-130">Property</span></span>|<span data-ttu-id="6e354-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e354-131">Type</span></span>|<span data-ttu-id="6e354-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e354-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e354-133">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="6e354-133">defaultLanguageTag</span></span>|<span data-ttu-id="6e354-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e354-134">String</span></span>|<span data-ttu-id="6e354-135">Idioma padrão do [microsoft.graph.termstore.store](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="6e354-135">Default language of the [microsoft.graph.termstore.store](../resources/termstore-store.md)</span></span>|
|<span data-ttu-id="6e354-136">languageTags</span><span class="sxs-lookup"><span data-stu-id="6e354-136">languageTags</span></span>|<span data-ttu-id="6e354-137">Coleção String</span><span class="sxs-lookup"><span data-stu-id="6e354-137">String collection</span></span>|<span data-ttu-id="6e354-138">Idiomas disponíveis na [microsoft.graph.termstore.store](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="6e354-138">Available languages in the [microsoft.graph.termstore.store](../resources/termstore-store.md)</span></span>|



## <a name="response"></a><span data-ttu-id="6e354-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e354-139">Response</span></span>

<span data-ttu-id="6e354-140">Se bem-sucedido, este método retorna `200 OK` um código de resposta e um objeto de [armazenamento](../resources/termstore-store.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e354-140">If successful, this method returns a `200 OK` response code and an updated [store](../resources/termstore-store.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e354-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6e354-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6e354-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e354-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6e354-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e354-143">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="6e354-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e354-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e354-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e354-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="6e354-146">C#</span><span class="sxs-lookup"><span data-stu-id="6e354-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-store-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6e354-147">Java</span><span class="sxs-lookup"><span data-stu-id="6e354-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-store-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6e354-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e354-148">Response</span></span>
<span data-ttu-id="6e354-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6e354-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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



