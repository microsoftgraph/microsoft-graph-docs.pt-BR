---
title: trustFrameworkPolicy
description: Na política de estrutura de confiança do Azure AD B2C é chamada de políticas personalizadas. Isso descreve as operações disponíveis em um objeto trustFrameworkPolicy para o locatário.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3160ce5ec75c0b65def8aed44ad89032cd293dee
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345460"
---
# <a name="trustframeworkpolicy-resource-type"></a><span data-ttu-id="d8a9e-104">tipo de recurso trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="d8a9e-104">trustFrameworkPolicy resource type</span></span>

> <span data-ttu-id="d8a9e-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d8a9e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8a9e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d8a9e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d8a9e-107">Representa uma diretiva de [estrutura de confiança](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) (também chamada de [política personalizada](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom)) no [Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview).</span><span class="sxs-lookup"><span data-stu-id="d8a9e-107">Represents a [Trust Framework](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) policy (also called [custom policy](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom)) in [Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview).</span></span> <span data-ttu-id="d8a9e-108">Uma política de estrutura de confiança fornece controle total sobre as viagens do usuário.</span><span class="sxs-lookup"><span data-stu-id="d8a9e-108">A Trust Framework policy gives full control over the user journeys.</span></span> <span data-ttu-id="d8a9e-109">Use-o para:</span><span class="sxs-lookup"><span data-stu-id="d8a9e-109">Use it to:</span></span>

* <span data-ttu-id="d8a9e-110">Personalize as experiências de inscrição e inscrição totalmente.</span><span class="sxs-lookup"><span data-stu-id="d8a9e-110">Customize the sign-up and sign-in experiences fully.</span></span>
* <span data-ttu-id="d8a9e-111">Federar para qualquer provedor SAML, Open ID Connect ou OAuth2 Identity Provider.</span><span class="sxs-lookup"><span data-stu-id="d8a9e-111">Federate to any SAML, Open ID Connect, or OAuth2 identity provider.</span></span>
* <span data-ttu-id="d8a9e-112">Integre-se com outros sistemas ou armazenamentos de dados do usuário chamando pontos de extremidade REST.</span><span class="sxs-lookup"><span data-stu-id="d8a9e-112">Integrate with other systems or user data stores by calling REST endpoints.</span></span>
* <span data-ttu-id="d8a9e-113">Transforme declarações e personalize tokens emitidos para o aplicativo de terceira parte confiável.</span><span class="sxs-lookup"><span data-stu-id="d8a9e-113">Transform claims and customize tokens issued to the relying party application.</span></span>

<span data-ttu-id="d8a9e-114">Para obter mais informações, consulte [Custom Policies in Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom).</span><span class="sxs-lookup"><span data-stu-id="d8a9e-114">For more information, see [Custom policies in Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom).</span></span>

## <a name="methods"></a><span data-ttu-id="d8a9e-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="d8a9e-115">Methods</span></span>

| <span data-ttu-id="d8a9e-116">Método</span><span class="sxs-lookup"><span data-stu-id="d8a9e-116">Method</span></span>       | <span data-ttu-id="d8a9e-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d8a9e-117">Return Type</span></span>  |<span data-ttu-id="d8a9e-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8a9e-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8a9e-119">Criar trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="d8a9e-119">Create trustFrameworkPolicy</span></span>](../api/trustframework-post-trustframeworkpolicy.md)|<span data-ttu-id="d8a9e-120">trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="d8a9e-120">trustFrameworkPolicy</span></span>|<span data-ttu-id="d8a9e-121">Criar um novo trustFrameworkPolicy.</span><span class="sxs-lookup"><span data-stu-id="d8a9e-121">Create a new trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="d8a9e-122">Obter trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="d8a9e-122">Get trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-get.md) |<span data-ttu-id="d8a9e-123">trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="d8a9e-123">trustFrameworkPolicy</span></span>|<span data-ttu-id="d8a9e-124">Ler as propriedades de um trustFrameworkPolicy existente.</span><span class="sxs-lookup"><span data-stu-id="d8a9e-124">Read properties of an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="d8a9e-125">Listar trustFrameworkPolicies</span><span class="sxs-lookup"><span data-stu-id="d8a9e-125">List trustFrameworkPolicies</span></span>](../api/trustframework-list-trustframeworkpolicies.md)|<span data-ttu-id="d8a9e-126">coleção trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="d8a9e-126">trustFrameworkPolicy collection</span></span>|<span data-ttu-id="d8a9e-127">Listar todos os trustFrameworkPolicies configurados em um locatário.</span><span class="sxs-lookup"><span data-stu-id="d8a9e-127">List all trustFrameworkPolicies configured in a tenant.</span></span>|
|[<span data-ttu-id="d8a9e-128">Atualizar ou criar trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="d8a9e-128">Update or create trustFrameworkPolicy</span></span>](../api/trustframework-put-trustframeworkpolicy.md)|<span data-ttu-id="d8a9e-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d8a9e-129">None</span></span>|<span data-ttu-id="d8a9e-130">Atualize um trustFrameworkPolicy existente.</span><span class="sxs-lookup"><span data-stu-id="d8a9e-130">Update an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="d8a9e-131">Excluir trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="d8a9e-131">Delete trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-delete.md)|<span data-ttu-id="d8a9e-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d8a9e-132">None</span></span>|<span data-ttu-id="d8a9e-133">Excluir um trustFrameworkPolicy existente.</span><span class="sxs-lookup"><span data-stu-id="d8a9e-133">Delete an existing trustFrameworkPolicy.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8a9e-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8a9e-134">Properties</span></span>

|<span data-ttu-id="d8a9e-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8a9e-135">Property</span></span>|<span data-ttu-id="d8a9e-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8a9e-136">Type</span></span>|<span data-ttu-id="d8a9e-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8a9e-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8a9e-138">id</span><span class="sxs-lookup"><span data-stu-id="d8a9e-138">id</span></span>|<span data-ttu-id="d8a9e-139">String</span><span class="sxs-lookup"><span data-stu-id="d8a9e-139">String</span></span>|<span data-ttu-id="d8a9e-140">A ID da política.</span><span class="sxs-lookup"><span data-stu-id="d8a9e-140">The ID of the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8a9e-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8a9e-141">JSON representation</span></span>

<span data-ttu-id="d8a9e-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8a9e-142">The following is a JSON representation of the resource.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d8a9e-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="d8a9e-143">See also</span></span>

- <span data-ttu-id="d8a9e-144">[trustFrameworkPolicy esquema](https://docs.microsoft.com/en-us/azure/active-directory-b2c/trustframeworkpolicy) para obter informações sobre os elementos do esquema.</span><span class="sxs-lookup"><span data-stu-id="d8a9e-144">[trustFrameworkPolicy schema](https://docs.microsoft.com/en-us/azure/active-directory-b2c/trustframeworkpolicy) for information about the schema elements.</span></span>  
- [<span data-ttu-id="d8a9e-145">trustFrameworkPolicy. xsd</span><span class="sxs-lookup"><span data-stu-id="d8a9e-145">trustFrameworkPolicy.xsd</span></span>](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)
