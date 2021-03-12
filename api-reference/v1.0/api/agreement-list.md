---
title: Listar contratos
description: Recupere uma lista de objetos de contrato.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: c4b0a56d258e0b67eb5561b9e9ff529b4ed311e8
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722520"
---
# <a name="list-agreements"></a><span data-ttu-id="eb73f-103">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="eb73f-103">List agreements</span></span>

<span data-ttu-id="eb73f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb73f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eb73f-105">Recupere uma lista de objetos [de](../resources/agreement.md) contrato.</span><span class="sxs-lookup"><span data-stu-id="eb73f-105">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="eb73f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="eb73f-106">Permissions</span></span>
<span data-ttu-id="eb73f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb73f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb73f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb73f-109">Permission type</span></span>                        | <span data-ttu-id="eb73f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb73f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb73f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb73f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb73f-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb73f-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="eb73f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb73f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb73f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb73f-114">Not supported.</span></span> |
|<span data-ttu-id="eb73f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb73f-115">Application</span></span>                            | <span data-ttu-id="eb73f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb73f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb73f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb73f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb73f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eb73f-118">Optional query parameters</span></span>
<span data-ttu-id="eb73f-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eb73f-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb73f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb73f-120">Request headers</span></span>
| <span data-ttu-id="eb73f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="eb73f-121">Name</span></span>         | <span data-ttu-id="eb73f-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb73f-122">Type</span></span>        | <span data-ttu-id="eb73f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb73f-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="eb73f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb73f-124">Authorization</span></span> | <span data-ttu-id="eb73f-125">string</span><span class="sxs-lookup"><span data-stu-id="eb73f-125">string</span></span> | <span data-ttu-id="eb73f-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb73f-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb73f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb73f-128">Request body</span></span>
<span data-ttu-id="eb73f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb73f-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="eb73f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb73f-130">Response</span></span>
<span data-ttu-id="eb73f-131">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [de](../resources/agreement.md) contrato no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb73f-131">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="eb73f-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eb73f-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="eb73f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb73f-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/termsOfUse/agreements
```

### <a name="response"></a><span data-ttu-id="eb73f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb73f-134">Response</span></span>
><span data-ttu-id="eb73f-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="eb73f-135">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
      "displayName": "Sample ToU",
      "isViewingBeforeAcceptanceRequired": true,
      "id": "093b947f-8363-4979-a47d-4c52b33ee1be"
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
