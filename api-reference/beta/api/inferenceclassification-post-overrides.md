---
title: Criar inferenceClassificationOverride
description: 'Criar uma substituição de caixa de entrada destaques para um remetente identificado por um endereço SMTP. Mensagens futuras desse endereço SMTP serão consistentemente classificadas '
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: b4165a9e299a75cfa2260b6b79ce0aff6ed6647a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326195"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="618c7-104">Criar inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="618c7-104">Create inferenceClassificationOverride</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="618c7-105">Criar uma substituição de [caixa de entrada destaques](../resources/manage-focused-inbox.md) para um remetente identificado por um endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="618c7-105">Create a [Focused Inbox](../resources/manage-focused-inbox.md) override for a sender identified by an SMTP address.</span></span> <span data-ttu-id="618c7-106">Mensagens futuras desse endereço SMTP serão consistentemente classificadas conforme especificado na substituição.</span><span class="sxs-lookup"><span data-stu-id="618c7-106">Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="618c7-107">**Observação**</span><span class="sxs-lookup"><span data-stu-id="618c7-107">**Note**</span></span>

- <span data-ttu-id="618c7-108">Se já existir uma substituição com o mesmo endereço SMTP, os campos de **classificação** e **nome** dessa substituição serão atualizados com os valores fornecidos.</span><span class="sxs-lookup"><span data-stu-id="618c7-108">If an override already exists with the same SMTP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="618c7-109">O número máximo de substituições com suporte para uma caixa de correio é 1000, com base nos endereços SMTP exclusivos do remetente.</span><span class="sxs-lookup"><span data-stu-id="618c7-109">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="618c7-110">A operação POST dá suporte à criação de apenas uma substituição de cada vez.</span><span class="sxs-lookup"><span data-stu-id="618c7-110">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="618c7-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="618c7-111">Permissions</span></span>
<span data-ttu-id="618c7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="618c7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="618c7-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="618c7-114">Permission type</span></span>      | <span data-ttu-id="618c7-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="618c7-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="618c7-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="618c7-116">Delegated (work or school account)</span></span> | <span data-ttu-id="618c7-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="618c7-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="618c7-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="618c7-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="618c7-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="618c7-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="618c7-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="618c7-120">Application</span></span> | <span data-ttu-id="618c7-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="618c7-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="618c7-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="618c7-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="618c7-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="618c7-123">Request headers</span></span>
| <span data-ttu-id="618c7-124">Nome</span><span class="sxs-lookup"><span data-stu-id="618c7-124">Name</span></span>       | <span data-ttu-id="618c7-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="618c7-125">Type</span></span> | <span data-ttu-id="618c7-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="618c7-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="618c7-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="618c7-127">Authorization</span></span>  | <span data-ttu-id="618c7-128">string</span><span class="sxs-lookup"><span data-stu-id="618c7-128">string</span></span>  | <span data-ttu-id="618c7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="618c7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="618c7-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="618c7-131">Content-Type</span></span> | <span data-ttu-id="618c7-132">string</span><span class="sxs-lookup"><span data-stu-id="618c7-132">string</span></span>  | <span data-ttu-id="618c7-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="618c7-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="618c7-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="618c7-135">Request body</span></span>
<span data-ttu-id="618c7-136">No corpo da solicitação, forneça uma representação JSON do objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).</span><span class="sxs-lookup"><span data-stu-id="618c7-136">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="618c7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="618c7-137">Response</span></span>

<span data-ttu-id="618c7-138">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="618c7-138">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="618c7-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="618c7-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="618c7-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="618c7-140">Request</span></span>
<span data-ttu-id="618c7-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="618c7-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="618c7-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="618c7-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_inferenceclassificationoverride_from_inferenceclassification"
}-->
```http
POST https://graph.microsoft.com/beta/me/inferenceClassification/overrides
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="618c7-143">C#</span><span class="sxs-lookup"><span data-stu-id="618c7-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-inferenceclassificationoverride-from-inferenceclassification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="618c7-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="618c7-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-inferenceclassificationoverride-from-inferenceclassification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="618c7-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="618c7-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-inferenceclassificationoverride-from-inferenceclassification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="618c7-146">Java</span><span class="sxs-lookup"><span data-stu-id="618c7-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-inferenceclassificationoverride-from-inferenceclassification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="618c7-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="618c7-147">Response</span></span>
<span data-ttu-id="618c7-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="618c7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
