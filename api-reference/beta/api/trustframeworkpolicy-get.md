---
title: Obter trustFrameworkPolicy
description: Esta operação recupera um conteúdo existente do trustFrameworkPolicy de um locatário do Azure AD B2C.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e4e0a10c0a4c230c172230eecfce177deb4a4d91
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536982"
---
# <a name="get-trustframeworkpolicy"></a><span data-ttu-id="d470e-103">Obter trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="d470e-103">Get trustFrameworkPolicy</span></span>

><span data-ttu-id="d470e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d470e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d470e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d470e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d470e-106">Recupere o conteúdo de um [trustFrameworkPolicy](../resources/trustframeworkpolicy.md)existente.</span><span class="sxs-lookup"><span data-stu-id="d470e-106">Retrieve the contents of an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d470e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d470e-107">Permissions</span></span>

<span data-ttu-id="d470e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d470e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="d470e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d470e-110">Permission type</span></span>      | <span data-ttu-id="d470e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d470e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d470e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d470e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d470e-113">Policy. Read. TrustFramework, Policy. Read. All</span><span class="sxs-lookup"><span data-stu-id="d470e-113">Policy.Read.TrustFramework, Policy.Read.All</span></span>|
|<span data-ttu-id="d470e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d470e-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d470e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d470e-115">Not supported.</span></span>|
|<span data-ttu-id="d470e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d470e-116">Application</span></span>|<span data-ttu-id="d470e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d470e-117">Not supported.</span></span>|

<span data-ttu-id="d470e-118">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="d470e-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="d470e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d470e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d470e-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d470e-120">Optional query parameters</span></span>

<span data-ttu-id="d470e-121">Este método oferece suporte `$select` aos `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d470e-121">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d470e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d470e-122">Request headers</span></span>

|<span data-ttu-id="d470e-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d470e-123">Name</span></span>|<span data-ttu-id="d470e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d470e-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d470e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d470e-125">Authorization</span></span>|<span data-ttu-id="d470e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d470e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d470e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d470e-128">Request body</span></span>

<span data-ttu-id="d470e-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d470e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d470e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d470e-130">Response</span></span>

<span data-ttu-id="d470e-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma representação XML do [trustFrameworkPolicy](../resources/trustFrameworkpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d470e-131">If successful, this method returns a `200 OK` response code and an XML representation of the [trustFrameworkPolicy](../resources/trustFrameworkpolicy.md) in the response body.</span></span>  

><span data-ttu-id="d470e-132">**Observação:** o tipo de conteúdo de resposta `application/xml`será.</span><span class="sxs-lookup"><span data-stu-id="d470e-132">**Note:** the response content type will be `application/xml`.</span></span>

## <a name="example"></a><span data-ttu-id="d470e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d470e-133">Example</span></span>

<span data-ttu-id="d470e-134">O exemplo a seguir recupera um **trustFrameworkPolicy**específico.</span><span class="sxs-lookup"><span data-stu-id="d470e-134">The following example retrieves a specific **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="d470e-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d470e-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_trustFramework"
}-->
```http
https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_Test/$value
```

##### <a name="response"></a><span data-ttu-id="d470e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d470e-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFramework.policy"
} -->
```http
HTTP/1.1 200 OK
Content-Type application/xml
<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_Test" PublicPolicyUri="http://tenantName.onmicrosoft.com/B2C_1A_Test">
    .....
    ....
    <!---PolicyContent-->
    ....
    ....
</TrustFrameworkPolicy>
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get trustFramework policy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
