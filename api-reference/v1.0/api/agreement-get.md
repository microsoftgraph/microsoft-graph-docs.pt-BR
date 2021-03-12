---
title: Obter contrato
description: Recupere as propriedades e as relações de um objeto de contrato.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 0218eeb4be68ded4d6e644ac0998be563c239b83
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722522"
---
# <a name="get-agreement"></a><span data-ttu-id="87795-103">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="87795-103">Get agreement</span></span>

<span data-ttu-id="87795-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87795-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="87795-105">Recupere as propriedades e as relações de um [objeto de](../resources/agreement.md) contrato.</span><span class="sxs-lookup"><span data-stu-id="87795-105">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="87795-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="87795-106">Permissions</span></span>
<span data-ttu-id="87795-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87795-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87795-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87795-109">Permission type</span></span>                        | <span data-ttu-id="87795-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87795-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="87795-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87795-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="87795-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="87795-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="87795-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87795-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87795-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87795-114">Not supported.</span></span> |
|<span data-ttu-id="87795-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87795-115">Application</span></span>                            | <span data-ttu-id="87795-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87795-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87795-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87795-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87795-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="87795-118">Optional query parameters</span></span>
<span data-ttu-id="87795-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="87795-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87795-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87795-120">Request headers</span></span>
| <span data-ttu-id="87795-121">Nome</span><span class="sxs-lookup"><span data-stu-id="87795-121">Name</span></span>         | <span data-ttu-id="87795-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="87795-122">Type</span></span>        | <span data-ttu-id="87795-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="87795-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="87795-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="87795-124">Authorization</span></span> | <span data-ttu-id="87795-125">string</span><span class="sxs-lookup"><span data-stu-id="87795-125">string</span></span> | <span data-ttu-id="87795-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87795-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87795-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87795-128">Request body</span></span>
<span data-ttu-id="87795-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87795-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="87795-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="87795-130">Response</span></span>
<span data-ttu-id="87795-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [agreement](../resources/agreement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87795-131">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87795-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87795-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="87795-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87795-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/termsOfUse/agreements/093b947f-8363-4979-a47d-4c52b33ee1be?$expand=files
```

### <a name="response"></a><span data-ttu-id="87795-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="87795-134">Response</span></span>
><span data-ttu-id="87795-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87795-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value",
  "files": [
    {
      "id": "093b947f-8363-4979-a47d-4c52b33ee1be",
      "language": "en",
      "fileName": "TOU.pdf",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
