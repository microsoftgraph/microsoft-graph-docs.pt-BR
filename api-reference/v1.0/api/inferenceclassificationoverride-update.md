---
title: Atualizar inferenceclassificationoverride
description: 'Altere o campo **classifyAs** de uma substituição conforme especificado. '
localization_priority: Normal
ms.openlocfilehash: dbb2553e0461d616abd9aa3e529f7b3e8c5023fb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273371"
---
# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="a79c5-103">Atualizar inferenceclassificationoverride</span><span class="sxs-lookup"><span data-stu-id="a79c5-103">Update inferenceclassificationoverride</span></span>

<span data-ttu-id="a79c5-104">Altere o campo **classifyAs** de uma substituição conforme especificado.</span><span class="sxs-lookup"><span data-stu-id="a79c5-104">Change the **classifyAs** field of an override as specified.</span></span> 

<span data-ttu-id="a79c5-105">Você não pode usar PATCH para alterar outros campos em uma instância de [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).</span><span class="sxs-lookup"><span data-stu-id="a79c5-105">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) instance.</span></span> 

<span data-ttu-id="a79c5-106">Se houver uma substituição de um remetente e o remetente alterar seu nome de exibição, você poderá usar [POST](inferenceclassification-post-overrides.md) para forçar uma atualização para o campo de nome em uma substituição existente.</span><span class="sxs-lookup"><span data-stu-id="a79c5-106">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification-post-overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="a79c5-107">Se houver uma substituição de um remetente e o remetente alterar seu endereço SMTP, [excluir](inferenceclassificationoverride-delete.md) a substituição existente e [criar](inferenceclassification-post-overrides.md) uma nova com o novo endereço SMTP será a única maneira de "atualizar" a substituição deste remetente.</span><span class="sxs-lookup"><span data-stu-id="a79c5-107">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride-delete.md) the existing override and [creating](inferenceclassification-post-overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="a79c5-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a79c5-108">Permissions</span></span>
<span data-ttu-id="a79c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a79c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a79c5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a79c5-111">Permission type</span></span>      | <span data-ttu-id="a79c5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a79c5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a79c5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a79c5-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a79c5-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a79c5-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a79c5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a79c5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a79c5-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a79c5-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a79c5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a79c5-117">Application</span></span> | <span data-ttu-id="a79c5-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a79c5-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a79c5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a79c5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a79c5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a79c5-120">Request headers</span></span>
| <span data-ttu-id="a79c5-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a79c5-121">Name</span></span>       | <span data-ttu-id="a79c5-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="a79c5-122">Type</span></span> | <span data-ttu-id="a79c5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a79c5-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a79c5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a79c5-124">Authorization</span></span>  | <span data-ttu-id="a79c5-125">string</span><span class="sxs-lookup"><span data-stu-id="a79c5-125">string</span></span>  | <span data-ttu-id="a79c5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a79c5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a79c5-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a79c5-128">Content-Type</span></span> | <span data-ttu-id="a79c5-129">string</span><span class="sxs-lookup"><span data-stu-id="a79c5-129">string</span></span>  | <span data-ttu-id="a79c5-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a79c5-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a79c5-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a79c5-132">Request body</span></span>
<span data-ttu-id="a79c5-p104">No corpo da solicitação, forneça o novo valor para **classifyAs**. Para obter o melhor desempenho, não inclua valores existentes que não estão sendo alterados.</span><span class="sxs-lookup"><span data-stu-id="a79c5-p104">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="a79c5-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a79c5-135">Property</span></span>     | <span data-ttu-id="a79c5-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="a79c5-136">Type</span></span>   |<span data-ttu-id="a79c5-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="a79c5-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a79c5-138">classifyAs</span><span class="sxs-lookup"><span data-stu-id="a79c5-138">classifyAs</span></span>|<span data-ttu-id="a79c5-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a79c5-139">string</span></span>| <span data-ttu-id="a79c5-140">Representa como classificar as mensagens recebidas de um remetente específico.</span><span class="sxs-lookup"><span data-stu-id="a79c5-140">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="a79c5-141">Os valores possíveis são: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="a79c5-141">The possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="a79c5-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a79c5-142">Response</span></span>

<span data-ttu-id="a79c5-143">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e o objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a79c5-143">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a79c5-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a79c5-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a79c5-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a79c5-145">Request</span></span>
<span data-ttu-id="a79c5-146">O exemplo a seguir altera a substituição para o endereço SMTP randiw@adatum.onmicrosoft.com de `other` para `focused`.</span><span class="sxs-lookup"><span data-stu-id="a79c5-146">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>

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
##### <a name="response"></a><span data-ttu-id="a79c5-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="a79c5-147">Response</span></span>
<span data-ttu-id="a79c5-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a79c5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a79c5-151">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a79c5-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a79c5-152">C#</span><span class="sxs-lookup"><span data-stu-id="a79c5-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_inferenceclassificationoverride-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a79c5-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="a79c5-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_inferenceclassificationoverride-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a79c5-154">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a79c5-154">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_inferenceclassificationoverride-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update inferenceclassificationoverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/inferenceclassificationoverride-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/inferenceclassificationoverride-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/inferenceclassificationoverride-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
