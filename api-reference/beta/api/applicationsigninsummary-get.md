---
title: Obter applicationSignInSummary
description: Recupere as propriedades e os relacionamentos de um objeto **applicationSigninSummary** .
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f10264ccdf6312c08ac2d64adeaa1c874707d350
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32639968"
---
# <a name="get-applicationsigninsummary"></a><span data-ttu-id="a3fb2-103">Obter applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="a3fb2-103">Get applicationSignInSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3fb2-104">Recupere as propriedades e os relacionamentos de um objeto [applicationSigninSummary](../resources/applicationsigninsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="a3fb2-104">Retrieve the properties and relationships of an [applicationSigninSummary](../resources/applicationsigninsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3fb2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a3fb2-105">Permissions</span></span>
<span data-ttu-id="a3fb2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a3fb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="a3fb2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3fb2-108">Permission type</span></span>      | <span data-ttu-id="a3fb2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3fb2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3fb2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3fb2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a3fb2-111">Report. Read. All</span><span class="sxs-lookup"><span data-stu-id="a3fb2-111">Report.Read.All</span></span> |
|<span data-ttu-id="a3fb2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3fb2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3fb2-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a3fb2-113">Not supported</span></span>   |
|<span data-ttu-id="a3fb2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3fb2-114">Application</span></span> | <span data-ttu-id="a3fb2-115">Report. Read. All</span><span class="sxs-lookup"><span data-stu-id="a3fb2-115">Report.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a3fb2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3fb2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
reports/getAzureADApplicationSignInSummary(period='{period}')
```

## <a name="function-parameters"></a><span data-ttu-id="a3fb2-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="a3fb2-117">Function parameters</span></span>

| <span data-ttu-id="a3fb2-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a3fb2-118">Parameter</span></span> | <span data-ttu-id="a3fb2-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3fb2-119">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="a3fb2-120">ponto</span><span class="sxs-lookup"><span data-stu-id="a3fb2-120">period</span></span> | <span data-ttu-id="a3fb2-121">`D7` (Últimos sete dias) ou `D30` (últimos 30 dias); outros valores geram erros.</span><span class="sxs-lookup"><span data-stu-id="a3fb2-121">Either `D7` (last seven days) or `D30` (last 30 days); other values generate errors.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="a3fb2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3fb2-122">Request headers</span></span>
| <span data-ttu-id="a3fb2-123">Nome</span><span class="sxs-lookup"><span data-stu-id="a3fb2-123">Name</span></span>      |<span data-ttu-id="a3fb2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3fb2-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a3fb2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3fb2-125">Authorization</span></span> | <span data-ttu-id="a3fb2-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a3fb2-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3fb2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3fb2-127">Request body</span></span>
<span data-ttu-id="a3fb2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a3fb2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3fb2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3fb2-129">Response</span></span>
<span data-ttu-id="a3fb2-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [applicationSignInSummary](../resources/applicationsigninsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3fb2-130">If successful, this method returns a `200 OK` response code and an [applicationSignInSummary](../resources/applicationsigninsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3fb2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3fb2-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a3fb2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3fb2-132">Request</span></span>
<span data-ttu-id="a3fb2-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3fb2-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applicationsigninsummary"
}-->
```http
https://graph.microsoft.com/beta/reports/getAzureADApplicationSignInSummary(period='D7')
```
### <a name="response"></a><span data-ttu-id="a3fb2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3fb2-134">Response</span></span>
<span data-ttu-id="a3fb2-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a3fb2-135">The following is an example of the response.</span></span> 

><span data-ttu-id="a3fb2-136">**Observação:** O objeto Response mostrado aqui mmight ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="a3fb2-136">**Note:** The response object shown here mmight be shortened for readability.</span></span> <span data-ttu-id="a3fb2-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3fb2-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationSignInSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "appId": "appId-value",
  "appDisplayName": "appDisplayName-value",
  "successfulSignInCount": 99,
  "failedSignInCount": 99,
  "successPercentage": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
