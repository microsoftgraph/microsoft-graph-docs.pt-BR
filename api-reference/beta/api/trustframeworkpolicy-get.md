---
title: Obter trustFrameworkPolicy
description: Esta operação recupera um conteúdo existente do trustFrameworkPolicy de um locatário do Azure AD B2C.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a8d7354175c9f49d7c39c1e16115fdcbadb3ba98
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43215858"
---
# <a name="get-trustframeworkpolicy"></a><span data-ttu-id="9bddd-103">Obter trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="9bddd-103">Get trustFrameworkPolicy</span></span>

<span data-ttu-id="9bddd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bddd-104">Namespace: microsoft.graph</span></span>

><span data-ttu-id="9bddd-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9bddd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bddd-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9bddd-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9bddd-107">Recupere o conteúdo de um [trustFrameworkPolicy](../resources/trustframeworkpolicy.md)existente.</span><span class="sxs-lookup"><span data-stu-id="9bddd-107">Retrieve the contents of an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9bddd-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="9bddd-108">Permissions</span></span>

<span data-ttu-id="9bddd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9bddd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="9bddd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bddd-111">Permission type</span></span>      | <span data-ttu-id="9bddd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9bddd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bddd-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bddd-113">Delegated (work or school account)</span></span>| <span data-ttu-id="9bddd-114">Policy. Read. All, Policy. ReadWrite. TrustFramework</span><span class="sxs-lookup"><span data-stu-id="9bddd-114">Policy.Read.All, Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="9bddd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bddd-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="9bddd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bddd-116">Not supported.</span></span>|
|<span data-ttu-id="9bddd-117">Application</span><span class="sxs-lookup"><span data-stu-id="9bddd-117">Application</span></span>|<span data-ttu-id="9bddd-118">Policy. Read. All, Policy. ReadWrite. TrustFramework</span><span class="sxs-lookup"><span data-stu-id="9bddd-118">Policy.Read.All, Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="9bddd-119">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="9bddd-119">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="9bddd-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bddd-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9bddd-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9bddd-121">Optional query parameters</span></span>

<span data-ttu-id="9bddd-122">Este método oferece suporte `$select` aos `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9bddd-122">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9bddd-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bddd-123">Request headers</span></span>

|<span data-ttu-id="9bddd-124">Nome</span><span class="sxs-lookup"><span data-stu-id="9bddd-124">Name</span></span>|<span data-ttu-id="9bddd-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bddd-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="9bddd-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bddd-126">Authorization</span></span>|<span data-ttu-id="9bddd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bddd-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bddd-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9bddd-129">Request body</span></span>

<span data-ttu-id="9bddd-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9bddd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bddd-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bddd-131">Response</span></span>

<span data-ttu-id="9bddd-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma representação XML do [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bddd-132">If successful, this method returns a `200 OK` response code and an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) in the response body.</span></span>  

><span data-ttu-id="9bddd-133">**Observação:** o tipo de conteúdo de resposta `application/xml`será.</span><span class="sxs-lookup"><span data-stu-id="9bddd-133">**Note:** the response content type will be `application/xml`.</span></span>

## <a name="example"></a><span data-ttu-id="9bddd-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bddd-134">Example</span></span>

<span data-ttu-id="9bddd-135">O exemplo a seguir recupera um **trustFrameworkPolicy**específico.</span><span class="sxs-lookup"><span data-stu-id="9bddd-135">The following example retrieves a specific **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="9bddd-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bddd-136">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_trustFramework"
}-->
```http
GET https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_Test/$value
```

##### <a name="response"></a><span data-ttu-id="9bddd-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bddd-137">Response</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/xml

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
