---
title: Substituições de lista
description: Obtenha as substituições de caixa de entrada focalizados em que um usuário tiver configurado para sempre classificar mensagens de determinados remetentes em meios específicos.
localization_priority: Normal
ms.openlocfilehash: a49d47e39caff5c00981d02551b0eeb564239f73
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511916"
---
# <a name="list-overrides"></a><span data-ttu-id="7bf01-103">Substituições de lista</span><span class="sxs-lookup"><span data-stu-id="7bf01-103">List overrides</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bf01-104">Obtenha as substituições de [Caixa de entrada focalizados em](../resources/manage-focused-inbox.md) que um usuário tiver configurado para sempre classificar mensagens de determinados remetentes em meios específicos.</span><span class="sxs-lookup"><span data-stu-id="7bf01-104">Get the [Focused Inbox](../resources/manage-focused-inbox.md) overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="7bf01-p101">Cada substituição corresponde a um endereço SMTP de um remetente. Inicialmente, um usuário não tem quaisquer substituições.</span><span class="sxs-lookup"><span data-stu-id="7bf01-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="7bf01-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7bf01-107">Permissions</span></span>
<span data-ttu-id="7bf01-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bf01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bf01-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bf01-110">Permission type</span></span>      | <span data-ttu-id="7bf01-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7bf01-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bf01-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bf01-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7bf01-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7bf01-113">Mail.Read</span></span>    |
|<span data-ttu-id="7bf01-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7bf01-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bf01-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7bf01-115">Mail.Read</span></span>    |
|<span data-ttu-id="7bf01-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bf01-116">Application</span></span> | <span data-ttu-id="7bf01-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7bf01-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bf01-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7bf01-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="7bf01-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7bf01-119">Request headers</span></span>
| <span data-ttu-id="7bf01-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7bf01-120">Name</span></span>       | <span data-ttu-id="7bf01-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bf01-121">Type</span></span> | <span data-ttu-id="7bf01-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bf01-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7bf01-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7bf01-123">Authorization</span></span>  | <span data-ttu-id="7bf01-124">string</span><span class="sxs-lookup"><span data-stu-id="7bf01-124">string</span></span>  | <span data-ttu-id="7bf01-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bf01-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bf01-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7bf01-127">Request body</span></span>
<span data-ttu-id="7bf01-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7bf01-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bf01-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bf01-129">Response</span></span>

<span data-ttu-id="7bf01-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7bf01-130">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7bf01-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7bf01-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7bf01-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bf01-132">Request</span></span>
<span data-ttu-id="7bf01-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7bf01-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/beta/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="7bf01-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bf01-134">Response</span></span>
<span data-ttu-id="7bf01-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7bf01-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List overrides",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/inferenceclassification-list-overrides.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
