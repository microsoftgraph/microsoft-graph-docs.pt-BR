---
title: Criar inferenceClassificationOverride
description: 'Crie uma substituição para um remetente identificado por um endereço SMTP. As mensagens futuras desse endereço SMTP serão classificadas consistentemente '
ms.openlocfilehash: f068984598ce841b2e7af52c1ed1d25c0e101d10
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006785"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="dfbff-104">Criar inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="dfbff-104">Create inferenceClassificationOverride</span></span>

<span data-ttu-id="dfbff-p102">Crie uma substituição para um remetente identificado por um endereço SMTP. Mensagens futuras desse endereço SMTP serão consistentemente classificadas conforme especificado na substituição.</span><span class="sxs-lookup"><span data-stu-id="dfbff-p102">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="dfbff-107">**Observação**</span><span class="sxs-lookup"><span data-stu-id="dfbff-107">**Note**</span></span>

- <span data-ttu-id="dfbff-108">Se já existir uma substituição com o mesmo endereço STMP, os campos **classifyAs** e **name** da substituição serão atualizados com os valores fornecidos.</span><span class="sxs-lookup"><span data-stu-id="dfbff-108">If an override already exists with the same STMP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="dfbff-109">O número máximo de substituições com suporte para uma caixa de correio é 1000, com base nos endereços SMTP exclusivos do remetente.</span><span class="sxs-lookup"><span data-stu-id="dfbff-109">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="dfbff-110">A operação POST dá suporte à criação de apenas uma substituição de cada vez.</span><span class="sxs-lookup"><span data-stu-id="dfbff-110">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfbff-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="dfbff-111">Permissions</span></span>
<span data-ttu-id="dfbff-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfbff-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfbff-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfbff-114">Permission type</span></span>      | <span data-ttu-id="dfbff-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dfbff-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfbff-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfbff-116">Delegated (work or school account)</span></span> | <span data-ttu-id="dfbff-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfbff-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dfbff-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfbff-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfbff-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfbff-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dfbff-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfbff-120">Application</span></span> | <span data-ttu-id="dfbff-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfbff-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfbff-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfbff-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="dfbff-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfbff-123">Request headers</span></span>
| <span data-ttu-id="dfbff-124">Nome</span><span class="sxs-lookup"><span data-stu-id="dfbff-124">Name</span></span>       | <span data-ttu-id="dfbff-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="dfbff-125">Type</span></span> | <span data-ttu-id="dfbff-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfbff-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dfbff-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfbff-127">Authorization</span></span>  | <span data-ttu-id="dfbff-128">string</span><span class="sxs-lookup"><span data-stu-id="dfbff-128">string</span></span>  | <span data-ttu-id="dfbff-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfbff-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dfbff-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dfbff-131">Content-Type</span></span> | <span data-ttu-id="dfbff-132">string</span><span class="sxs-lookup"><span data-stu-id="dfbff-132">string</span></span>  | <span data-ttu-id="dfbff-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfbff-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfbff-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfbff-135">Request body</span></span>
<span data-ttu-id="dfbff-136">No corpo da solicitação, forneça uma representação JSON do objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).</span><span class="sxs-lookup"><span data-stu-id="dfbff-136">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dfbff-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfbff-137">Response</span></span>

<span data-ttu-id="dfbff-138">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfbff-138">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfbff-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dfbff-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dfbff-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfbff-140">Request</span></span>
<span data-ttu-id="dfbff-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfbff-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="dfbff-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfbff-142">Response</span></span>
<span data-ttu-id="dfbff-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfbff-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->