---
title: Criar trustFrameworkPolicy
description: Essa operação cria um novo objeto trustFrameworkPolicy em um locatário do Azure AD B2C.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 39dd9cbc14ae0dc6040618619595dd4cceb0dadc
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734462"
---
# <a name="create-trustframeworkpolicy"></a><span data-ttu-id="d2f85-103">Criar trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="d2f85-103">Create trustFrameworkPolicy</span></span>

> <span data-ttu-id="d2f85-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d2f85-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2f85-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d2f85-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d2f85-106">Criar novo objeto [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="d2f85-106">Create new [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2f85-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2f85-107">Permissions</span></span>

<span data-ttu-id="d2f85-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d2f85-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="d2f85-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2f85-110">Permission type</span></span>      | <span data-ttu-id="d2f85-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2f85-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2f85-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2f85-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d2f85-113">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="d2f85-113">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="d2f85-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2f85-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d2f85-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2f85-115">Not supported.</span></span>|
|<span data-ttu-id="d2f85-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2f85-116">Application</span></span>|<span data-ttu-id="d2f85-117">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="d2f85-117">Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="d2f85-118">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="d2f85-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="d2f85-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2f85-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /trustFramework/policies
```

## <a name="request-headers"></a><span data-ttu-id="d2f85-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2f85-120">Request headers</span></span>

|<span data-ttu-id="d2f85-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d2f85-121">Name</span></span>|<span data-ttu-id="d2f85-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2f85-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d2f85-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2f85-123">Authorization</span></span>|<span data-ttu-id="d2f85-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2f85-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d2f85-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2f85-126">Content-Type</span></span>|<span data-ttu-id="d2f85-127">Application/XML.</span><span class="sxs-lookup"><span data-stu-id="d2f85-127">application/xml.</span></span> <span data-ttu-id="d2f85-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2f85-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2f85-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2f85-129">Request body</span></span>

<span data-ttu-id="d2f85-130">No corpo da solicitação, forneça uma representação XML do objeto [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="d2f85-130">In the request body, provide an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span> <span data-ttu-id="d2f85-131">O tipo de conteúdo deve ser `application/xml`.</span><span class="sxs-lookup"><span data-stu-id="d2f85-131">The content type must be `application/xml`.</span></span>

## <a name="response"></a><span data-ttu-id="d2f85-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2f85-132">Response</span></span>

<span data-ttu-id="d2f85-133">Se bem-sucedido, este método retorna um `201 Created` código de resposta e um objeto [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2f85-133">If successful, this method returns a `201 Created` response code and [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object in the response body.</span></span> <span data-ttu-id="d2f85-134">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="d2f85-134">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="d2f85-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2f85-135">Example</span></span>

<span data-ttu-id="d2f85-136">O exemplo a seguir cria um **trustFrameworkPolicy**.</span><span class="sxs-lookup"><span data-stu-id="d2f85-136">The following example creates a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="d2f85-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2f85-137">Request</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "name": "create_trustframeworkpolicy_from_trustframeworkpolicy"
}-->
```http
POST https://graph.microsoft.com/beta/trustFramework/policies
Content-Type: application/xml

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```

##### <a name="response"></a><span data-ttu-id="d2f85-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2f85-138">Response</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/xml
Location: /trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base/

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base" PublicPolicyUri="http://tenantName.onmicrosoft.com/B2C_1A_Test">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
