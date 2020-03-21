---
title: Obter identitySecurityDefaultsEnforcementPolicy
description: Recupere as propriedades e os relacionamentos do objeto identitysecuritydefaultsenforcementpolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c2ae06cd13c4c9f7401e839d8ac570710ac9e41c
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895473"
---
# <a name="get-identitysecuritydefaultsenforcementpolicy"></a><span data-ttu-id="b6360-103">Obter identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="b6360-103">Get identitySecurityDefaultsEnforcementPolicy</span></span>

<span data-ttu-id="b6360-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6360-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6360-105">Recupere as propriedades de um objeto [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="b6360-105">Retrieve the properties of an [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6360-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6360-106">Permissions</span></span>

<span data-ttu-id="b6360-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6360-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b6360-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6360-109">Permission type</span></span>                        | <span data-ttu-id="b6360-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6360-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b6360-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6360-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b6360-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6360-112">Policy.Read.All</span></span> |
| <span data-ttu-id="b6360-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6360-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6360-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6360-114">Not supported.</span></span> |
| <span data-ttu-id="b6360-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6360-115">Application</span></span>                            | <span data-ttu-id="b6360-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6360-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6360-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6360-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/identitySecurityDefaultsEnforcementPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6360-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b6360-118">Optional query parameters</span></span>

<span data-ttu-id="b6360-119">Este método oferece suporte `select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b6360-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="b6360-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b6360-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6360-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6360-121">Request headers</span></span>

| <span data-ttu-id="b6360-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b6360-122">Name</span></span>      |<span data-ttu-id="b6360-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6360-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b6360-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6360-124">Authorization</span></span> | <span data-ttu-id="b6360-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6360-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6360-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6360-127">Request body</span></span>

<span data-ttu-id="b6360-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6360-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6360-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6360-129">Response</span></span>

<span data-ttu-id="b6360-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6360-130">If successful, this method returns a `200 OK` response code and the requested [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b6360-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b6360-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b6360-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6360-132">Request</span></span>

<span data-ttu-id="b6360-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6360-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identitysecuritydefaultsenforcementpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/policies/identitySecurityDefaultsEnforcementPolicy
```

### <a name="response"></a><span data-ttu-id="b6360-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6360-134">Response</span></span>

<span data-ttu-id="b6360-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b6360-135">The following is an example of the response.</span></span>

> <span data-ttu-id="b6360-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6360-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/identitySecurityDefaultsEnforcementPolicy",
  "description": "Security defaults is a set of basic identity security mechanisms recommended by Microsoft. When enabled, these recommendations will be automatically enforced in your organization. Administrators and users will be better protected from common identity related attacks.",
  "displayName": "Security Defaults",
  "id": "00000000-0000-0000-0000-000000000005",
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identitySecurityDefaultsEnforcementPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
