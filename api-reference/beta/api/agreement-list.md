---
title: Listar contratos
description: Recupere uma lista de objetos de contrato.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 13bc5308f12ce83e03177f79df1264cca9b35bf1
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471572"
---
# <a name="list-agreements"></a><span data-ttu-id="b9cb5-103">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="b9cb5-103">List agreements</span></span>

<span data-ttu-id="b9cb5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9cb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9cb5-105">Recupere uma lista de objetos [de](../resources/agreement.md) contrato.</span><span class="sxs-lookup"><span data-stu-id="b9cb5-105">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b9cb5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b9cb5-106">Permissions</span></span>
<span data-ttu-id="b9cb5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9cb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9cb5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9cb5-109">Permission type</span></span>                        | <span data-ttu-id="b9cb5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9cb5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9cb5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9cb5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9cb5-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9cb5-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="b9cb5-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9cb5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9cb5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9cb5-114">Not supported.</span></span> |
|<span data-ttu-id="b9cb5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9cb5-115">Application</span></span>                            | <span data-ttu-id="b9cb5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9cb5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9cb5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9cb5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="b9cb5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9cb5-118">Request headers</span></span>
| <span data-ttu-id="b9cb5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b9cb5-119">Name</span></span>         | <span data-ttu-id="b9cb5-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9cb5-120">Type</span></span>        | <span data-ttu-id="b9cb5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9cb5-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b9cb5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9cb5-122">Authorization</span></span> | <span data-ttu-id="b9cb5-123">string</span><span class="sxs-lookup"><span data-stu-id="b9cb5-123">string</span></span> | <span data-ttu-id="b9cb5-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9cb5-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9cb5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9cb5-126">Request body</span></span>
<span data-ttu-id="b9cb5-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9cb5-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b9cb5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9cb5-128">Response</span></span>
<span data-ttu-id="b9cb5-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [de](../resources/agreement.md) contrato no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9cb5-129">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b9cb5-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9cb5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9cb5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9cb5-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements
```

##### <a name="response"></a><span data-ttu-id="b9cb5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9cb5-132">Response</span></span>
><span data-ttu-id="b9cb5-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9cb5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "value": [
    {
      "displayName": "displayName-value",
      "isViewingBeforeAcceptanceRequired": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreements",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
