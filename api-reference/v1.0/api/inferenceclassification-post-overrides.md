---
title: Criar inferenceClassificationOverride
description: 'Crie uma substituição para um remetente identificado por um endereço SMTP. Mensagens futuras desse endereço SMTP serão consistentemente classificadas '
localization_priority: Normal
ms.openlocfilehash: c4871e8af96a10387df4e1f04690a9adf2a75d30
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613831"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="94ce5-104">Criar inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="94ce5-104">Create inferenceClassificationOverride</span></span>

<span data-ttu-id="94ce5-p102">Crie uma substituição para um remetente identificado por um endereço SMTP. Mensagens futuras desse endereço SMTP serão consistentemente classificadas conforme especificado na substituição.</span><span class="sxs-lookup"><span data-stu-id="94ce5-p102">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="94ce5-107">**Observação**</span><span class="sxs-lookup"><span data-stu-id="94ce5-107">**Note**</span></span>

- <span data-ttu-id="94ce5-108">Se já existir uma substituição com o mesmo endereço STMP, os campos **classifyAs** e **name** da substituição serão atualizados com os valores fornecidos.</span><span class="sxs-lookup"><span data-stu-id="94ce5-108">If an override already exists with the same STMP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="94ce5-109">O número máximo de substituições com suporte para uma caixa de correio é 1000, com base nos endereços SMTP exclusivos do remetente.</span><span class="sxs-lookup"><span data-stu-id="94ce5-109">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="94ce5-110">A operação POST dá suporte à criação de apenas uma substituição de cada vez.</span><span class="sxs-lookup"><span data-stu-id="94ce5-110">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="94ce5-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="94ce5-111">Permissions</span></span>
<span data-ttu-id="94ce5-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94ce5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94ce5-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94ce5-114">Permission type</span></span>      | <span data-ttu-id="94ce5-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94ce5-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94ce5-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94ce5-116">Delegated (work or school account)</span></span> | <span data-ttu-id="94ce5-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94ce5-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="94ce5-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94ce5-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94ce5-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94ce5-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="94ce5-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94ce5-120">Application</span></span> | <span data-ttu-id="94ce5-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94ce5-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="94ce5-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94ce5-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="94ce5-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94ce5-123">Request headers</span></span>
| <span data-ttu-id="94ce5-124">Nome</span><span class="sxs-lookup"><span data-stu-id="94ce5-124">Name</span></span>       | <span data-ttu-id="94ce5-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="94ce5-125">Type</span></span> | <span data-ttu-id="94ce5-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="94ce5-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="94ce5-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="94ce5-127">Authorization</span></span>  | <span data-ttu-id="94ce5-128">string</span><span class="sxs-lookup"><span data-stu-id="94ce5-128">string</span></span>  | <span data-ttu-id="94ce5-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94ce5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="94ce5-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94ce5-131">Content-Type</span></span> | <span data-ttu-id="94ce5-132">string</span><span class="sxs-lookup"><span data-stu-id="94ce5-132">string</span></span>  | <span data-ttu-id="94ce5-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94ce5-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94ce5-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94ce5-135">Request body</span></span>
<span data-ttu-id="94ce5-136">No corpo da solicitação, forneça uma representação JSON do objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).</span><span class="sxs-lookup"><span data-stu-id="94ce5-136">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="94ce5-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="94ce5-137">Response</span></span>

<span data-ttu-id="94ce5-138">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94ce5-138">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94ce5-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94ce5-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94ce5-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94ce5-140">Request</span></span>
<span data-ttu-id="94ce5-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94ce5-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="94ce5-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="94ce5-142">Response</span></span>
<span data-ttu-id="94ce5-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94ce5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="94ce5-146">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="94ce5-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="94ce5-147">Basic</span><span class="sxs-lookup"><span data-stu-id="94ce5-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_inferenceclassificationoverride_from_inferenceclassification-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="94ce5-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94ce5-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_inferenceclassificationoverride_from_inferenceclassification-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/inferenceclassification-post-overrides.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/inferenceclassification-post-overrides.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
