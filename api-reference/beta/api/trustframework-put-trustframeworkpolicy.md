---
title: Atualizar trustFrameworkPolicy
description: 'Esta operação atualiza um objeto trustFrameworkPolicy existente ou, se houver algum, ele cria um. '
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: de2327489d6606c40fe55934d333f2fd2f9c0b44
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536975"
---
# <a name="update-or-create-trustframeworkpolicy"></a><span data-ttu-id="f32c4-103">Atualizar ou criar trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="f32c4-103">Update or create trustFrameworkPolicy</span></span>

><span data-ttu-id="f32c4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f32c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f32c4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f32c4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f32c4-106">Atualize um [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) existente ou crie um se ele não existir.</span><span class="sxs-lookup"><span data-stu-id="f32c4-106">Update an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) or create one if it does not exist.</span></span>

## <a name="permissions"></a><span data-ttu-id="f32c4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f32c4-107">Permissions</span></span>

<span data-ttu-id="f32c4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f32c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="f32c4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f32c4-110">Permission type</span></span>      | <span data-ttu-id="f32c4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f32c4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f32c4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f32c4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f32c4-113">Policy. ReadWrite. TrustFramework, Policy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f32c4-113">Policy.ReadWrite.TrustFramework, Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="f32c4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f32c4-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f32c4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f32c4-115">Not supported.</span></span>|
|<span data-ttu-id="f32c4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f32c4-116">Application</span></span>|<span data-ttu-id="f32c4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f32c4-117">Not supported.</span></span>|

<span data-ttu-id="f32c4-118">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="f32c4-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="f32c4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f32c4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /trustFramework/policies/{id}/$value
```

## <a name="request-headers"></a><span data-ttu-id="f32c4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f32c4-120">Request headers</span></span>

|<span data-ttu-id="f32c4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f32c4-121">Name</span></span>|<span data-ttu-id="f32c4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f32c4-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f32c4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f32c4-123">Authorization</span></span>|<span data-ttu-id="f32c4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f32c4-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f32c4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f32c4-126">Content-Type</span></span>|<span data-ttu-id="f32c4-127">Application/XML.</span><span class="sxs-lookup"><span data-stu-id="f32c4-127">application/xml.</span></span> <span data-ttu-id="f32c4-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f32c4-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f32c4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f32c4-129">Request body</span></span>

<span data-ttu-id="f32c4-130">No corpo da solicitação, forneça uma representação XML do objeto [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="f32c4-130">In the request body, provide an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span> 

><span data-ttu-id="f32c4-131">**Observação:** o tipo de conteúdo deve `application/xml`ser.</span><span class="sxs-lookup"><span data-stu-id="f32c4-131">**Note:** the content type must be `application/xml`.</span></span>

## <a name="response"></a><span data-ttu-id="f32c4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f32c4-132">Response</span></span>

<span data-ttu-id="f32c4-133">A resposta será uma das seguintes:</span><span class="sxs-lookup"><span data-stu-id="f32c4-133">The response will be one of the following:</span></span>
- <span data-ttu-id="f32c4-134">Se existir um [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) , uma solicitação bem-sucedida retornará um `200 OK` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="f32c4-134">If a [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) exists, a successful request returns a `200 OK` response code.</span></span>
- <span data-ttu-id="f32c4-135">Se não existir um [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) , uma solicitação com êxito retornará um `201 Created` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="f32c4-135">If a [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) does not exist, a successful request returns a `201 Created` response code.</span></span>
- <span data-ttu-id="f32c4-136">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="f32c4-136">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="f32c4-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f32c4-137">Example</span></span>

<span data-ttu-id="f32c4-138">O exemplo a seguir atualiza um **trustFrameworkPolicy**.</span><span class="sxs-lookup"><span data-stu-id="f32c4-138">The following example updates a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="f32c4-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f32c4-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_trustframeworkpolicy"
}-->
```http
PUT https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base/$value
Content-Type:application/xml
<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```

##### <a name="response"></a><span data-ttu-id="f32c4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f32c4-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
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
