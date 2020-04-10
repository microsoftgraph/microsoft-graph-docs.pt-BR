---
title: Criar trustFrameworkPolicy
description: Essa operação cria um novo objeto trustFrameworkPolicy em um locatário do Azure AD B2C.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b3e06b35d838817e3214ea10d22c11fe8d19d59f
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43215914"
---
# <a name="create-trustframeworkpolicy"></a><span data-ttu-id="9fb97-103">Criar trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="9fb97-103">Create trustFrameworkPolicy</span></span>

<span data-ttu-id="9fb97-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fb97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fb97-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9fb97-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9fb97-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9fb97-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9fb97-107">Criar novo objeto [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="9fb97-107">Create new [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fb97-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="9fb97-108">Permissions</span></span>

<span data-ttu-id="9fb97-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9fb97-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="9fb97-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9fb97-111">Permission type</span></span>      | <span data-ttu-id="9fb97-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9fb97-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fb97-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9fb97-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9fb97-114">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="9fb97-114">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="9fb97-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9fb97-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="9fb97-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fb97-116">Not supported.</span></span>|
|<span data-ttu-id="9fb97-117">Application</span><span class="sxs-lookup"><span data-stu-id="9fb97-117">Application</span></span>|<span data-ttu-id="9fb97-118">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="9fb97-118">Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="9fb97-119">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="9fb97-119">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="9fb97-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9fb97-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /trustFramework/policies
```

## <a name="request-headers"></a><span data-ttu-id="9fb97-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9fb97-121">Request headers</span></span>

|<span data-ttu-id="9fb97-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9fb97-122">Name</span></span>|<span data-ttu-id="9fb97-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fb97-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="9fb97-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9fb97-124">Authorization</span></span>|<span data-ttu-id="9fb97-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fb97-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9fb97-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9fb97-127">Content-Type</span></span>|<span data-ttu-id="9fb97-128">Application/XML.</span><span class="sxs-lookup"><span data-stu-id="9fb97-128">application/xml.</span></span> <span data-ttu-id="9fb97-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fb97-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fb97-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9fb97-130">Request body</span></span>

<span data-ttu-id="9fb97-131">No corpo da solicitação, forneça uma representação XML do objeto [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="9fb97-131">In the request body, provide an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span> <span data-ttu-id="9fb97-132">O tipo de conteúdo deve ser `application/xml`.</span><span class="sxs-lookup"><span data-stu-id="9fb97-132">The content type must be `application/xml`.</span></span>

## <a name="response"></a><span data-ttu-id="9fb97-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fb97-133">Response</span></span>

<span data-ttu-id="9fb97-134">Se bem-sucedido, este método retorna um `201 Created` código de resposta e um objeto [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9fb97-134">If successful, this method returns a `201 Created` response code and [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object in the response body.</span></span> <span data-ttu-id="9fb97-135">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="9fb97-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="9fb97-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9fb97-136">Example</span></span>

<span data-ttu-id="9fb97-137">O exemplo a seguir cria um **trustFrameworkPolicy**.</span><span class="sxs-lookup"><span data-stu-id="9fb97-137">The following example creates a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="9fb97-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fb97-138">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="9fb97-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fb97-139">Response</span></span>

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
