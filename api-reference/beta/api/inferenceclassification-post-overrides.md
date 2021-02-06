---
title: Criar inferenceClassificationOverride
description: 'Criar uma substituição da Caixa de Entrada Destaques para um remetente identificado por um endereço SMTP. Mensagens futuras desse endereço SMTP serão consistentemente classificadas '
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: ''
ms.openlocfilehash: 82f309e1d4da5e8482679c61470a91dcad8d9a04
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130339"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="18162-104">Criar inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="18162-104">Create inferenceClassificationOverride</span></span>

<span data-ttu-id="18162-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18162-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18162-106">Crie uma [substituição da Caixa de](../resources/manage-focused-inbox.md) Entrada Focada para um remetente identificado por um endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="18162-106">Create a [Focused Inbox](../resources/manage-focused-inbox.md) override for a sender identified by an SMTP address.</span></span> <span data-ttu-id="18162-107">Mensagens futuras desse endereço SMTP serão consistentemente classificadas conforme especificado na substituição.</span><span class="sxs-lookup"><span data-stu-id="18162-107">Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="18162-108">**Observação**</span><span class="sxs-lookup"><span data-stu-id="18162-108">**Note**</span></span>

- <span data-ttu-id="18162-109">Se já existir uma substituição com o mesmo endereço SMTP, **os campos classifyAs** e **name** dessa substituição serão atualizados com os valores fornecidos.</span><span class="sxs-lookup"><span data-stu-id="18162-109">If an override already exists with the same SMTP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="18162-110">O número máximo de substituições com suporte para uma caixa de correio é 1000, com base nos endereços SMTP exclusivos do remetente.</span><span class="sxs-lookup"><span data-stu-id="18162-110">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="18162-111">A operação POST dá suporte à criação de apenas uma substituição de cada vez.</span><span class="sxs-lookup"><span data-stu-id="18162-111">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="18162-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="18162-112">Permissions</span></span>
<span data-ttu-id="18162-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18162-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18162-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18162-115">Permission type</span></span>      | <span data-ttu-id="18162-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18162-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18162-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18162-117">Delegated (work or school account)</span></span> | <span data-ttu-id="18162-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18162-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="18162-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18162-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18162-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18162-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="18162-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18162-121">Application</span></span> | <span data-ttu-id="18162-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18162-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="18162-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18162-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="18162-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18162-124">Request headers</span></span>
| <span data-ttu-id="18162-125">Nome</span><span class="sxs-lookup"><span data-stu-id="18162-125">Name</span></span>       | <span data-ttu-id="18162-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="18162-126">Type</span></span> | <span data-ttu-id="18162-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="18162-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="18162-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="18162-128">Authorization</span></span>  | <span data-ttu-id="18162-129">string</span><span class="sxs-lookup"><span data-stu-id="18162-129">string</span></span>  | <span data-ttu-id="18162-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18162-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18162-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18162-132">Content-Type</span></span> | <span data-ttu-id="18162-133">string</span><span class="sxs-lookup"><span data-stu-id="18162-133">string</span></span>  | <span data-ttu-id="18162-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18162-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18162-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18162-136">Request body</span></span>
<span data-ttu-id="18162-137">No corpo da solicitação, forneça uma representação JSON do objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).</span><span class="sxs-lookup"><span data-stu-id="18162-137">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="18162-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="18162-138">Response</span></span>

<span data-ttu-id="18162-139">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18162-139">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18162-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18162-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18162-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18162-141">Request</span></span>
<span data-ttu-id="18162-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18162-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="18162-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="18162-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="18162-144">C#</span><span class="sxs-lookup"><span data-stu-id="18162-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-inferenceclassificationoverride-from-inferenceclassification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18162-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18162-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-inferenceclassificationoverride-from-inferenceclassification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18162-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18162-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-inferenceclassificationoverride-from-inferenceclassification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18162-147">Java</span><span class="sxs-lookup"><span data-stu-id="18162-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-inferenceclassificationoverride-from-inferenceclassification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="18162-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="18162-148">Response</span></span>
<span data-ttu-id="18162-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18162-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


