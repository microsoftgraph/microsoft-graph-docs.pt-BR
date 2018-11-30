---
title: Substituições de lista
description: Obtenha as substituições de caixa de entrada focalizados em que um usuário tiver configurado para sempre classificar mensagens de determinados remetentes em meios específicos.
ms.openlocfilehash: 343faaacf47d16b723cd8aebc25a6df79ef7e3db
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040414"
---
# <a name="list-overrides"></a><span data-ttu-id="43bcd-103">Substituições de lista</span><span class="sxs-lookup"><span data-stu-id="43bcd-103">List overrides</span></span>

> <span data-ttu-id="43bcd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="43bcd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43bcd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="43bcd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="43bcd-106">Obtenha as substituições de [Caixa de entrada focalizados em](../resources/manage-focused-inbox.md) que um usuário tiver configurado para sempre classificar mensagens de determinados remetentes em meios específicos.</span><span class="sxs-lookup"><span data-stu-id="43bcd-106">Get the [Focused Inbox](../resources/manage-focused-inbox.md) overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="43bcd-p102">Cada substituição corresponde a um endereço SMTP de um remetente. Inicialmente, um usuário não tem quaisquer substituições.</span><span class="sxs-lookup"><span data-stu-id="43bcd-p102">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="43bcd-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="43bcd-109">Permissions</span></span>
<span data-ttu-id="43bcd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43bcd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43bcd-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43bcd-112">Permission type</span></span>      | <span data-ttu-id="43bcd-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43bcd-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43bcd-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43bcd-114">Delegated (work or school account)</span></span> | <span data-ttu-id="43bcd-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="43bcd-115">Mail.Read</span></span>    |
|<span data-ttu-id="43bcd-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43bcd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43bcd-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="43bcd-117">Mail.Read</span></span>    |
|<span data-ttu-id="43bcd-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43bcd-118">Application</span></span> | <span data-ttu-id="43bcd-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="43bcd-119">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="43bcd-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43bcd-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="43bcd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43bcd-121">Request headers</span></span>
| <span data-ttu-id="43bcd-122">Nome</span><span class="sxs-lookup"><span data-stu-id="43bcd-122">Name</span></span>       | <span data-ttu-id="43bcd-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="43bcd-123">Type</span></span> | <span data-ttu-id="43bcd-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="43bcd-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="43bcd-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="43bcd-125">Authorization</span></span>  | <span data-ttu-id="43bcd-126">string</span><span class="sxs-lookup"><span data-stu-id="43bcd-126">string</span></span>  | <span data-ttu-id="43bcd-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43bcd-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43bcd-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43bcd-129">Request body</span></span>
<span data-ttu-id="43bcd-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43bcd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43bcd-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="43bcd-131">Response</span></span>

<span data-ttu-id="43bcd-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43bcd-132">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="43bcd-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43bcd-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="43bcd-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43bcd-134">Request</span></span>
<span data-ttu-id="43bcd-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="43bcd-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/beta/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="43bcd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="43bcd-136">Response</span></span>
<span data-ttu-id="43bcd-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43bcd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "classifyAs": "focused",
      "senderEmailAddress": {
        "name": "Samantha Booth",
        "address": "samanthab@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
    },
    {
      "classifyAs": "other",
      "senderEmailAddress": {
        "name": "Randi Welch",
        "address": "randiw@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List overrides",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->