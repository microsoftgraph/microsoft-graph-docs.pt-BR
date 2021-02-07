---
title: Atualizar inferenceclassificationoverride
description: 'Altere o campo **classifyAs** de uma substituição conforme especificado. '
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 60625066f8da1c8ad0effeaad33a55a4b32dd81b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135188"
---
# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="c6922-103">Atualizar inferenceclassificationoverride</span><span class="sxs-lookup"><span data-stu-id="c6922-103">Update inferenceclassificationoverride</span></span>

<span data-ttu-id="c6922-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6922-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c6922-105">Altere o campo **classifyAs** de uma substituição conforme especificado.</span><span class="sxs-lookup"><span data-stu-id="c6922-105">Change the **classifyAs** field of an override as specified.</span></span>

<span data-ttu-id="c6922-106">Você não pode usar PATCH para alterar outros campos em uma instância de [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).</span><span class="sxs-lookup"><span data-stu-id="c6922-106">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) instance.</span></span>

<span data-ttu-id="c6922-107">Se houver uma substituição de um remetente e o remetente alterar seu nome de exibição, você poderá usar [POST](inferenceclassification-post-overrides.md) para forçar uma atualização para o campo de nome em uma substituição existente.</span><span class="sxs-lookup"><span data-stu-id="c6922-107">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification-post-overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="c6922-108">Se houver uma substituição de um remetente e o remetente alterar seu endereço SMTP, [excluir](inferenceclassificationoverride-delete.md) a substituição existente e [criar](inferenceclassification-post-overrides.md) uma nova com o novo endereço SMTP será a única maneira de "atualizar" a substituição deste remetente.</span><span class="sxs-lookup"><span data-stu-id="c6922-108">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride-delete.md) the existing override and [creating](inferenceclassification-post-overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6922-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="c6922-109">Permissions</span></span>
<span data-ttu-id="c6922-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6922-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6922-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6922-112">Permission type</span></span>      | <span data-ttu-id="c6922-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6922-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6922-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6922-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c6922-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6922-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c6922-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6922-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6922-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6922-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c6922-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6922-118">Application</span></span> | <span data-ttu-id="c6922-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6922-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6922-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6922-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c6922-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6922-121">Request headers</span></span>
| <span data-ttu-id="c6922-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c6922-122">Name</span></span>       | <span data-ttu-id="c6922-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6922-123">Type</span></span> | <span data-ttu-id="c6922-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6922-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c6922-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6922-125">Authorization</span></span>  | <span data-ttu-id="c6922-126">string</span><span class="sxs-lookup"><span data-stu-id="c6922-126">string</span></span>  | <span data-ttu-id="c6922-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6922-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c6922-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c6922-129">Content-Type</span></span> | <span data-ttu-id="c6922-130">string</span><span class="sxs-lookup"><span data-stu-id="c6922-130">string</span></span>  | <span data-ttu-id="c6922-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6922-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6922-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6922-133">Request body</span></span>
<span data-ttu-id="c6922-p104">No corpo da solicitação, forneça o novo valor para **classifyAs**. Para obter o melhor desempenho, não inclua valores existentes que não estão sendo alterados.</span><span class="sxs-lookup"><span data-stu-id="c6922-p104">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="c6922-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6922-136">Property</span></span>     | <span data-ttu-id="c6922-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6922-137">Type</span></span>   |<span data-ttu-id="c6922-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6922-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6922-139">classifyAs</span><span class="sxs-lookup"><span data-stu-id="c6922-139">classifyAs</span></span>|<span data-ttu-id="c6922-140">string</span><span class="sxs-lookup"><span data-stu-id="c6922-140">string</span></span>| <span data-ttu-id="c6922-141">Representa como classificar as mensagens recebidas de um remetente específico.</span><span class="sxs-lookup"><span data-stu-id="c6922-141">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="c6922-142">Os valores possíveis são: `focused` , `other` .</span><span class="sxs-lookup"><span data-stu-id="c6922-142">The possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="c6922-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6922-143">Response</span></span>

<span data-ttu-id="c6922-144">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e o objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6922-144">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c6922-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6922-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6922-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6922-146">Request</span></span>
<span data-ttu-id="c6922-147">O exemplo a seguir altera a substituição para o endereço SMTP randiw@adatum.onmicrosoft.com de `other` para `focused`.</span><span class="sxs-lookup"><span data-stu-id="c6922-147">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>


# <a name="http"></a>[<span data-ttu-id="c6922-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6922-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_inferenceclassificationoverride"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/{id}
Content-type: application/json

{
  "classifyAs": "focused"
}
```
# <a name="c"></a>[<span data-ttu-id="c6922-149">C#</span><span class="sxs-lookup"><span data-stu-id="c6922-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-inferenceclassificationoverride-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6922-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6922-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-inferenceclassificationoverride-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6922-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6922-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-inferenceclassificationoverride-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c6922-152">Java</span><span class="sxs-lookup"><span data-stu-id="c6922-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-inferenceclassificationoverride-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c6922-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6922-153">Response</span></span>
<span data-ttu-id="c6922-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6922-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Randi Welch",
    "address": "randiw@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update inferenceclassificationoverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

