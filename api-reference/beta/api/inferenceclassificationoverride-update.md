---
title: Atualizar inferenceClassificationOverride
description: 'Altere o **** campo classificas de uma substituição de caixa de entrada destaques, conforme especificado. '
localization_priority: Normal
ms.openlocfilehash: 83832c11f09afdfdb27c0020005870c945f4a28d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857462"
---
# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="10787-103">Atualizar inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="10787-103">Update inferenceClassificationOverride</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10787-104">Altere o \*\*\*\* campo classificas de uma substituição de [caixa de entrada destaques](../resources/manage-focused-inbox.md) , conforme especificado.</span><span class="sxs-lookup"><span data-stu-id="10787-104">Change the **classifyAs** field of a [Focused Inbox](../resources/manage-focused-inbox.md) override as specified.</span></span> 

<span data-ttu-id="10787-105">Você não pode usar PATCH para alterar outros campos em uma instância de [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).</span><span class="sxs-lookup"><span data-stu-id="10787-105">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) instance.</span></span> 

<span data-ttu-id="10787-106">Se houver uma substituição de um remetente e o remetente alterar seu nome de exibição, você poderá usar [POST](inferenceclassification-post-overrides.md) para forçar uma atualização para o campo de nome em uma substituição existente.</span><span class="sxs-lookup"><span data-stu-id="10787-106">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification-post-overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="10787-107">Se houver uma substituição de um remetente e o remetente alterar seu endereço SMTP, [excluir](inferenceclassificationoverride-delete.md) a substituição existente e [criar](inferenceclassification-post-overrides.md) uma nova com o novo endereço SMTP será a única maneira de "atualizar" a substituição deste remetente.</span><span class="sxs-lookup"><span data-stu-id="10787-107">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride-delete.md) the existing override and [creating](inferenceclassification-post-overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="10787-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="10787-108">Permissions</span></span>
<span data-ttu-id="10787-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10787-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10787-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10787-111">Permission type</span></span>      | <span data-ttu-id="10787-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="10787-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10787-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10787-113">Delegated (work or school account)</span></span> | <span data-ttu-id="10787-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10787-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="10787-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10787-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10787-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10787-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="10787-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10787-117">Application</span></span> | <span data-ttu-id="10787-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10787-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="10787-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10787-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="10787-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10787-120">Request headers</span></span>
| <span data-ttu-id="10787-121">Nome</span><span class="sxs-lookup"><span data-stu-id="10787-121">Name</span></span>       | <span data-ttu-id="10787-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="10787-122">Type</span></span> | <span data-ttu-id="10787-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="10787-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="10787-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="10787-124">Authorization</span></span>  | <span data-ttu-id="10787-125">string</span><span class="sxs-lookup"><span data-stu-id="10787-125">string</span></span>  | <span data-ttu-id="10787-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10787-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="10787-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10787-128">Content-Type</span></span> | <span data-ttu-id="10787-129">string</span><span class="sxs-lookup"><span data-stu-id="10787-129">string</span></span>  | <span data-ttu-id="10787-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10787-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10787-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10787-132">Request body</span></span>
<span data-ttu-id="10787-p104">No corpo da solicitação, forneça o novo valor para **classifyAs**. Para obter o melhor desempenho, não inclua valores existentes que não estão sendo alterados.</span><span class="sxs-lookup"><span data-stu-id="10787-p104">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="10787-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10787-135">Property</span></span>     | <span data-ttu-id="10787-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="10787-136">Type</span></span>   |<span data-ttu-id="10787-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="10787-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10787-138">classifyAs</span><span class="sxs-lookup"><span data-stu-id="10787-138">classifyAs</span></span>|<span data-ttu-id="10787-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10787-139">string</span></span>| <span data-ttu-id="10787-p105">Representa como classificar as mensagens recebidas de um remetente específico. Os valores possíveis são: `focused` e `other`.</span><span class="sxs-lookup"><span data-stu-id="10787-p105">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="10787-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="10787-142">Response</span></span>

<span data-ttu-id="10787-143">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e o objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10787-143">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="10787-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10787-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10787-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10787-145">Request</span></span>
<span data-ttu-id="10787-146">O exemplo a seguir altera a substituição para o endereço SMTP randiw@adatum.onmicrosoft.com de `other` para `focused`.</span><span class="sxs-lookup"><span data-stu-id="10787-146">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="10787-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="10787-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_inferenceclassificationoverride"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/inferenceClassification/overrides/{id}
Content-type: application/json

{
  "classifyAs": "focused"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="10787-148">C#</span><span class="sxs-lookup"><span data-stu-id="10787-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-inferenceclassificationoverride-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="10787-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="10787-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-inferenceclassificationoverride-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="10787-150">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="10787-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-inferenceclassificationoverride-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="10787-151">Java</span><span class="sxs-lookup"><span data-stu-id="10787-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-inferenceclassificationoverride-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="10787-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="10787-152">Response</span></span>
<span data-ttu-id="10787-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10787-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update inferenceclassificationoverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
