---
title: trustFrameworkPolicy
description: Na política de estrutura de confiança do Azure AD B2C é conhecida como políticas personalizadas. Isso descreve as operações disponíveis em um objeto trustFrameworkPolicy para o locatário.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a8bb9fc598613d48ac6b9bb34aa02d24872e6300
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442737"
---
# <a name="trustframeworkpolicy-resource-type"></a><span data-ttu-id="03110-104">Tipo de recurso trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="03110-104">trustFrameworkPolicy resource type</span></span>

<span data-ttu-id="03110-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03110-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03110-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="03110-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03110-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="03110-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="03110-108">Representa uma [política da Estrutura de Confiança](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) (também chamada de política [personalizada](/azure/active-directory-b2c/active-directory-b2c-overview-custom)) no [Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview).</span><span class="sxs-lookup"><span data-stu-id="03110-108">Represents a [Trust Framework](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) policy (also called [custom policy](/azure/active-directory-b2c/active-directory-b2c-overview-custom)) in [Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview).</span></span> <span data-ttu-id="03110-109">Uma política da Estrutura de Confiança dá controle total sobre as jornadas do usuário.</span><span class="sxs-lookup"><span data-stu-id="03110-109">A Trust Framework policy gives full control over the user journeys.</span></span> <span data-ttu-id="03110-110">Use-o para:</span><span class="sxs-lookup"><span data-stu-id="03110-110">Use it to:</span></span>

* <span data-ttu-id="03110-111">Personalize totalmente as experiências de assinatura e de login.</span><span class="sxs-lookup"><span data-stu-id="03110-111">Customize the sign-up and sign-in experiences fully.</span></span>
* <span data-ttu-id="03110-112">Federar para qualquer provedor de identidade SAML, Open ID Connect ou OAuth2.</span><span class="sxs-lookup"><span data-stu-id="03110-112">Federate to any SAML, Open ID Connect, or OAuth2 identity provider.</span></span>
* <span data-ttu-id="03110-113">Integre-se a outros sistemas ou armazenamentos de dados do usuário chamando pontos de extremidade REST.</span><span class="sxs-lookup"><span data-stu-id="03110-113">Integrate with other systems or user data stores by calling REST endpoints.</span></span>
* <span data-ttu-id="03110-114">Transforme declarações e personalize tokens emitidos para o aplicativo de terceiros de confiança.</span><span class="sxs-lookup"><span data-stu-id="03110-114">Transform claims and customize tokens issued to the relying party application.</span></span>

<span data-ttu-id="03110-115">Para obter mais informações, consulte [Políticas personalizadas no Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview-custom).</span><span class="sxs-lookup"><span data-stu-id="03110-115">For more information, see [Custom policies in Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview-custom).</span></span>

## <a name="methods"></a><span data-ttu-id="03110-116">Methods</span><span class="sxs-lookup"><span data-stu-id="03110-116">Methods</span></span>

| <span data-ttu-id="03110-117">Método</span><span class="sxs-lookup"><span data-stu-id="03110-117">Method</span></span>       | <span data-ttu-id="03110-118">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="03110-118">Return Type</span></span>  |<span data-ttu-id="03110-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="03110-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="03110-120">Criar trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="03110-120">Create trustFrameworkPolicy</span></span>](../api/trustframework-post-trustframeworkpolicy.md)|<span data-ttu-id="03110-121">trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="03110-121">trustFrameworkPolicy</span></span>|<span data-ttu-id="03110-122">Crie um novo trustFrameworkPolicy.</span><span class="sxs-lookup"><span data-stu-id="03110-122">Create a new trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="03110-123">Obter trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="03110-123">Get trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-get.md) |<span data-ttu-id="03110-124">trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="03110-124">trustFrameworkPolicy</span></span>|<span data-ttu-id="03110-125">Ler propriedades de um trustFrameworkPolicy existente.</span><span class="sxs-lookup"><span data-stu-id="03110-125">Read properties of an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="03110-126">Listar trustFrameworkPolicies</span><span class="sxs-lookup"><span data-stu-id="03110-126">List trustFrameworkPolicies</span></span>](../api/trustframework-list-trustframeworkpolicies.md)|<span data-ttu-id="03110-127">Coleção trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="03110-127">trustFrameworkPolicy collection</span></span>|<span data-ttu-id="03110-128">Listar todos os trustFrameworkPolicies configurados em um locatário.</span><span class="sxs-lookup"><span data-stu-id="03110-128">List all trustFrameworkPolicies configured in a tenant.</span></span>|
|[<span data-ttu-id="03110-129">Atualizar ou criar trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="03110-129">Update or create trustFrameworkPolicy</span></span>](../api/trustframework-put-trustframeworkpolicy.md)|<span data-ttu-id="03110-130">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="03110-130">None</span></span>|<span data-ttu-id="03110-131">Atualize um trustFrameworkPolicy existente.</span><span class="sxs-lookup"><span data-stu-id="03110-131">Update an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="03110-132">Excluir trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="03110-132">Delete trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-delete.md)|<span data-ttu-id="03110-133">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="03110-133">None</span></span>|<span data-ttu-id="03110-134">Exclua um trustFrameworkPolicy existente.</span><span class="sxs-lookup"><span data-stu-id="03110-134">Delete an existing trustFrameworkPolicy.</span></span>|

## <a name="properties"></a><span data-ttu-id="03110-135">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03110-135">Properties</span></span>

|<span data-ttu-id="03110-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03110-136">Property</span></span>|<span data-ttu-id="03110-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="03110-137">Type</span></span>|<span data-ttu-id="03110-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="03110-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03110-139">id</span><span class="sxs-lookup"><span data-stu-id="03110-139">id</span></span>|<span data-ttu-id="03110-140">String</span><span class="sxs-lookup"><span data-stu-id="03110-140">String</span></span>|<span data-ttu-id="03110-141">A ID da política.</span><span class="sxs-lookup"><span data-stu-id="03110-141">The ID of the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03110-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03110-142">JSON representation</span></span>

<span data-ttu-id="03110-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03110-143">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType":"microsoft.graph.entity",
  "keyProperty":"id",
  "isMediaEntity":true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy"
}-->
```json
{
   "id": "B2C_1A_Test"
}
```

## <a name="see-also"></a><span data-ttu-id="03110-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="03110-144">See also</span></span>

- <span data-ttu-id="03110-145">[esquema trustFrameworkPolicy](/azure/active-directory-b2c/trustframeworkpolicy) para obter informações sobre os elementos de esquema.</span><span class="sxs-lookup"><span data-stu-id="03110-145">[trustFrameworkPolicy schema](/azure/active-directory-b2c/trustframeworkpolicy) for information about the schema elements.</span></span>
- [<span data-ttu-id="03110-146">trustFrameworkPolicy.xsd</span><span class="sxs-lookup"><span data-stu-id="03110-146">trustFrameworkPolicy.xsd</span></span>](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)


