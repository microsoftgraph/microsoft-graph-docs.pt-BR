---
title: Criar inferenceClassificationOverride
description: 'Crie uma substituição para um remetente identificado por um endereço SMTP. Mensagens futuras desse endereço SMTP serão consistentemente classificadas '
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: cccfaa892f7dbfa444ddcba33d20d735ab29bde0
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806496"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="8c644-104">Criar inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="8c644-104">Create inferenceClassificationOverride</span></span>

<span data-ttu-id="8c644-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c644-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8c644-p102">Crie uma substituição para um remetente identificado por um endereço SMTP. Mensagens futuras desse endereço SMTP serão consistentemente classificadas conforme especificado na substituição.</span><span class="sxs-lookup"><span data-stu-id="8c644-p102">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="8c644-108">**Observação**</span><span class="sxs-lookup"><span data-stu-id="8c644-108">**Note**</span></span>

- <span data-ttu-id="8c644-109">Se já existir uma substituição com o mesmo endereço SMTP, os campos de **classificação** e **nome** dessa substituição serão atualizados com os valores fornecidos.</span><span class="sxs-lookup"><span data-stu-id="8c644-109">If an override already exists with the same SMTP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="8c644-110">O número máximo de substituições com suporte para uma caixa de correio é 1000, com base nos endereços SMTP exclusivos do remetente.</span><span class="sxs-lookup"><span data-stu-id="8c644-110">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="8c644-111">A operação POST dá suporte à criação de apenas uma substituição de cada vez.</span><span class="sxs-lookup"><span data-stu-id="8c644-111">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c644-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c644-112">Permissions</span></span>
<span data-ttu-id="8c644-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c644-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c644-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c644-115">Permission type</span></span>      | <span data-ttu-id="8c644-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c644-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c644-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c644-117">Delegated (work or school account)</span></span> | <span data-ttu-id="8c644-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c644-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8c644-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c644-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c644-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c644-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8c644-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c644-121">Application</span></span> | <span data-ttu-id="8c644-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c644-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c644-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c644-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="8c644-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c644-124">Request headers</span></span>
| <span data-ttu-id="8c644-125">Nome</span><span class="sxs-lookup"><span data-stu-id="8c644-125">Name</span></span>       | <span data-ttu-id="8c644-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c644-126">Type</span></span> | <span data-ttu-id="8c644-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c644-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8c644-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c644-128">Authorization</span></span>  | <span data-ttu-id="8c644-129">string</span><span class="sxs-lookup"><span data-stu-id="8c644-129">string</span></span>  | <span data-ttu-id="8c644-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c644-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c644-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c644-132">Content-Type</span></span> | <span data-ttu-id="8c644-133">string</span><span class="sxs-lookup"><span data-stu-id="8c644-133">string</span></span>  | <span data-ttu-id="8c644-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c644-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c644-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c644-136">Request body</span></span>
<span data-ttu-id="8c644-137">No corpo da solicitação, forneça uma representação JSON do objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).</span><span class="sxs-lookup"><span data-stu-id="8c644-137">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8c644-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c644-138">Response</span></span>

<span data-ttu-id="8c644-139">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c644-139">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c644-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c644-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c644-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c644-141">Request</span></span>
<span data-ttu-id="8c644-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c644-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8c644-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c644-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_inferenceclassificationoverride_from_inferenceclassification"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="8c644-144">C#</span><span class="sxs-lookup"><span data-stu-id="8c644-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-inferenceclassificationoverride-from-inferenceclassification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c644-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c644-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-inferenceclassificationoverride-from-inferenceclassification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c644-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c644-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-inferenceclassificationoverride-from-inferenceclassification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c644-147">Java</span><span class="sxs-lookup"><span data-stu-id="8c644-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-inferenceclassificationoverride-from-inferenceclassification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8c644-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c644-148">Response</span></span>
<span data-ttu-id="8c644-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c644-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
