---
title: Atualizar trustFrameworkPolicy
description: 'Essa operação atualiza um objeto trustFrameworkPolicy existente ou, se não existir, ele cria um. '
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2305c7dfde39d742ce1694c030f395f59f6fb7bb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443283"
---
# <a name="update-or-create-trustframeworkpolicy"></a><span data-ttu-id="3d88e-103">Atualizar ou criar trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="3d88e-103">Update or create trustFrameworkPolicy</span></span>

<span data-ttu-id="3d88e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d88e-104">Namespace: microsoft.graph</span></span>

><span data-ttu-id="3d88e-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3d88e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d88e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3d88e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3d88e-107">Atualize um [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) existente ou crie um se ele não existir.</span><span class="sxs-lookup"><span data-stu-id="3d88e-107">Update an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) or create one if it does not exist.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d88e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d88e-108">Permissions</span></span>

<span data-ttu-id="3d88e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3d88e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="3d88e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d88e-111">Permission type</span></span>      | <span data-ttu-id="3d88e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d88e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d88e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d88e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d88e-114">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="3d88e-114">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="3d88e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d88e-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3d88e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d88e-116">Not supported.</span></span>|
|<span data-ttu-id="3d88e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d88e-117">Application</span></span>|<span data-ttu-id="3d88e-118">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="3d88e-118">Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="3d88e-119">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="3d88e-119">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="3d88e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d88e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /trustFramework/policies/{id}/$value
```

## <a name="request-headers"></a><span data-ttu-id="3d88e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d88e-121">Request headers</span></span>

|<span data-ttu-id="3d88e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3d88e-122">Name</span></span>|<span data-ttu-id="3d88e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d88e-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3d88e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d88e-124">Authorization</span></span>|<span data-ttu-id="3d88e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d88e-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3d88e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3d88e-127">Content-Type</span></span>|<span data-ttu-id="3d88e-128">application/xml.</span><span class="sxs-lookup"><span data-stu-id="3d88e-128">application/xml.</span></span> <span data-ttu-id="3d88e-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d88e-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d88e-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d88e-130">Request body</span></span>

<span data-ttu-id="3d88e-131">No corpo da solicitação, forneça uma representação XML do [objeto trustFrameworkPolicy.](../resources/trustframeworkpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3d88e-131">In the request body, provide an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span> 

><span data-ttu-id="3d88e-132">**Observação:** o tipo de conteúdo deve ser `application/xml` .</span><span class="sxs-lookup"><span data-stu-id="3d88e-132">**Note:** the content type must be `application/xml`.</span></span>

## <a name="response"></a><span data-ttu-id="3d88e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d88e-133">Response</span></span>

<span data-ttu-id="3d88e-134">A resposta será uma das seguintes:</span><span class="sxs-lookup"><span data-stu-id="3d88e-134">The response will be one of the following:</span></span>
- <span data-ttu-id="3d88e-135">Se existir [um trustFrameworkPolicy,](../resources/trustframeworkpolicy.md) uma solicitação bem-sucedida retornará um `200 OK` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="3d88e-135">If a [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) exists, a successful request returns a `200 OK` response code.</span></span>
- <span data-ttu-id="3d88e-136">Se um [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) não existir, uma solicitação bem-sucedida retornará um `201 Created` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="3d88e-136">If a [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) does not exist, a successful request returns a `201 Created` response code.</span></span>
- <span data-ttu-id="3d88e-137">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="3d88e-137">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="3d88e-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d88e-138">Example</span></span>

<span data-ttu-id="3d88e-139">O exemplo a seguir atualiza **um trustFrameworkPolicy**.</span><span class="sxs-lookup"><span data-stu-id="3d88e-139">The following example updates a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="3d88e-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d88e-140">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "update_trustframeworkpolicy"
}-->
```http
PUT https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base/$value
Content-Type: application/xml

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```

##### <a name="response"></a><span data-ttu-id="3d88e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d88e-141">Response</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true
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
  "description": "Update trustframeworkpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


