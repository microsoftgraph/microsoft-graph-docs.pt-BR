---
title: Atualizar configurações
description: Atualize as configurações de todo o locatário para o serviço de impressão universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d9e17edaf303c1e62aef4211e080cbdf5d2d00cc
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948195"
---
# <a name="update-settings"></a><span data-ttu-id="e0c30-103">Atualizar configurações</span><span class="sxs-lookup"><span data-stu-id="e0c30-103">Update settings</span></span>

<span data-ttu-id="e0c30-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0c30-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0c30-105">Atualize as configurações de todo o locatário para o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="e0c30-105">Update tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0c30-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0c30-106">Permissions</span></span>
<span data-ttu-id="e0c30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0c30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e0c30-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="e0c30-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="e0c30-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0c30-110">Permission type</span></span> | <span data-ttu-id="e0c30-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0c30-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e0c30-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0c30-112">Delegated (work or school account)</span></span>| <span data-ttu-id="e0c30-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="e0c30-113">Users.Read.All</span></span> |
|<span data-ttu-id="e0c30-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0c30-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0c30-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0c30-115">Not Supported.</span></span>|
|<span data-ttu-id="e0c30-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0c30-116">Application</span></span>|<span data-ttu-id="e0c30-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0c30-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0c30-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0c30-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/settings
```

## <a name="optional-request-headers"></a><span data-ttu-id="e0c30-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="e0c30-119">Optional request headers</span></span>
| <span data-ttu-id="e0c30-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e0c30-120">Name</span></span>       | <span data-ttu-id="e0c30-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0c30-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e0c30-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0c30-122">Authorization</span></span> | <span data-ttu-id="e0c30-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0c30-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e0c30-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="e0c30-125">Content-type</span></span>  | <span data-ttu-id="e0c30-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0c30-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0c30-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0c30-128">Request body</span></span>
<span data-ttu-id="e0c30-129">No corpo da solicitação, forneça os valores para os campos de [configurações](../resources/printsettings.md) relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="e0c30-129">In the request body, supply the values for the relevant [printSettings](../resources/printsettings.md) fields that should be updated.</span></span> <span data-ttu-id="e0c30-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="e0c30-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e0c30-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e0c30-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e0c30-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0c30-132">Property</span></span>     | <span data-ttu-id="e0c30-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0c30-133">Type</span></span>        | <span data-ttu-id="e0c30-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0c30-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e0c30-135">documentConversionEnabled</span><span class="sxs-lookup"><span data-stu-id="e0c30-135">documentConversionEnabled</span></span>|<span data-ttu-id="e0c30-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0c30-136">Boolean</span></span>|<span data-ttu-id="e0c30-137">Especifica se a conversão de documentos está habilitada para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e0c30-137">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="e0c30-138">Se a conversão de documentos estiver habilitada, o serviço de impressão universal converterá automaticamente os documentos em um formato compatível com a impressora (por exemplo, XPS para PDF), quando necessário.</span><span class="sxs-lookup"><span data-stu-id="e0c30-138">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (for example, XPS to PDF) when needed.</span></span>|

## <a name="response"></a><span data-ttu-id="e0c30-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0c30-139">Response</span></span>
<span data-ttu-id="e0c30-140">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="e0c30-140">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0c30-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0c30-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0c30-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0c30-142">Request</span></span>
<span data-ttu-id="e0c30-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0c30-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0c30-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0c30-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_settings"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/settings
Content-type: application/json

{
  "documentConversionEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="e0c30-145">C#</span><span class="sxs-lookup"><span data-stu-id="e0c30-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0c30-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0c30-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0c30-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0c30-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e0c30-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0c30-148">Response</span></span>
<span data-ttu-id="e0c30-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e0c30-149">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printSettings"
} -->
```http
HTTP/1.1 204 NoContent
Content-length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
