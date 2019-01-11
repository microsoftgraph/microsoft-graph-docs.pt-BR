---
title: Obter contrato
description: Recupere as propriedades e relacionamentos de um objeto de contrato.
localization_priority: Normal
ms.openlocfilehash: 0ca4e941705fe716c3aa11a73c934c40deb279d4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818652"
---
# <a name="get-agreement"></a><span data-ttu-id="d7fa0-103">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="d7fa0-103">Get agreement</span></span>

> <span data-ttu-id="d7fa0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d7fa0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7fa0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d7fa0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d7fa0-106">Recupere as propriedades e relacionamentos de um objeto de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="d7fa0-106">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d7fa0-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="d7fa0-107">Permissions</span></span>
<span data-ttu-id="d7fa0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7fa0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7fa0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7fa0-110">Permission type</span></span>                        | <span data-ttu-id="d7fa0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d7fa0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7fa0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7fa0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d7fa0-113">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7fa0-113">Agreement.Read.All</span></span> |
|<span data-ttu-id="d7fa0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7fa0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7fa0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7fa0-115">Not supported.</span></span> |
|<span data-ttu-id="d7fa0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7fa0-116">Application</span></span>                            | <span data-ttu-id="d7fa0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7fa0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7fa0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7fa0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements/<id>
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="d7fa0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7fa0-119">Request headers</span></span>
| <span data-ttu-id="d7fa0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d7fa0-120">Name</span></span>         | <span data-ttu-id="d7fa0-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7fa0-121">Type</span></span>        | <span data-ttu-id="d7fa0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7fa0-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d7fa0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7fa0-123">Authorization</span></span> | <span data-ttu-id="d7fa0-124">string</span><span class="sxs-lookup"><span data-stu-id="d7fa0-124">string</span></span> | <span data-ttu-id="d7fa0-125">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="d7fa0-125">Bearer \{token\}.</span></span> <span data-ttu-id="d7fa0-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7fa0-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7fa0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7fa0-127">Request body</span></span>
<span data-ttu-id="d7fa0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d7fa0-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d7fa0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7fa0-129">Response</span></span>
<span data-ttu-id="d7fa0-130">Se tiver êxito, este método retornará um `200 OK` objeto de [contrato](../resources/agreement.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7fa0-130">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d7fa0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7fa0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7fa0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7fa0-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```http
GET https://graph.microsoft.com/beta/agreements/<id>?$expand=files
```
##### <a name="response"></a><span data-ttu-id="d7fa0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7fa0-133">Response</span></span>
><span data-ttu-id="d7fa0-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7fa0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
      "id": "id-value",
      "language": "en",
      "fileName": "TOU.pdf",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
