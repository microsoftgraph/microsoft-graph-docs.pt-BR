---
title: trustFrameworkPolicy
description: Na política de estrutura de confiança do Azure AD B2C é chamada de políticas personalizadas. Isso descreve as operações disponíveis em um objeto trustFrameworkPolicy para o locatário.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2cda564b353675d54305db5c0e6eaaa64682a7ef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519635"
---
# <a name="trustframeworkpolicy-resource-type"></a><span data-ttu-id="d7a59-104">tipo de recurso trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="d7a59-104">trustFrameworkPolicy resource type</span></span>

<span data-ttu-id="d7a59-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d7a59-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7a59-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d7a59-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7a59-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d7a59-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d7a59-108">Representa uma diretiva de [estrutura de confiança](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) (também chamada de [política personalizada](/azure/active-directory-b2c/active-directory-b2c-overview-custom)) no [Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview).</span><span class="sxs-lookup"><span data-stu-id="d7a59-108">Represents a [Trust Framework](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) policy (also called [custom policy](/azure/active-directory-b2c/active-directory-b2c-overview-custom)) in [Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview).</span></span> <span data-ttu-id="d7a59-109">Uma política de estrutura de confiança fornece controle total sobre as viagens do usuário.</span><span class="sxs-lookup"><span data-stu-id="d7a59-109">A Trust Framework policy gives full control over the user journeys.</span></span> <span data-ttu-id="d7a59-110">Use-o para:</span><span class="sxs-lookup"><span data-stu-id="d7a59-110">Use it to:</span></span>

* <span data-ttu-id="d7a59-111">Personalize as experiências de inscrição e inscrição totalmente.</span><span class="sxs-lookup"><span data-stu-id="d7a59-111">Customize the sign-up and sign-in experiences fully.</span></span>
* <span data-ttu-id="d7a59-112">Federar para qualquer provedor SAML, Open ID Connect ou OAuth2 Identity Provider.</span><span class="sxs-lookup"><span data-stu-id="d7a59-112">Federate to any SAML, Open ID Connect, or OAuth2 identity provider.</span></span>
* <span data-ttu-id="d7a59-113">Integre-se com outros sistemas ou armazenamentos de dados do usuário chamando pontos de extremidade REST.</span><span class="sxs-lookup"><span data-stu-id="d7a59-113">Integrate with other systems or user data stores by calling REST endpoints.</span></span>
* <span data-ttu-id="d7a59-114">Transforme declarações e personalize tokens emitidos para o aplicativo de terceira parte confiável.</span><span class="sxs-lookup"><span data-stu-id="d7a59-114">Transform claims and customize tokens issued to the relying party application.</span></span>

<span data-ttu-id="d7a59-115">Para obter mais informações, consulte [Custom Policies in Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview-custom).</span><span class="sxs-lookup"><span data-stu-id="d7a59-115">For more information, see [Custom policies in Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview-custom).</span></span>

## <a name="methods"></a><span data-ttu-id="d7a59-116">Métodos</span><span class="sxs-lookup"><span data-stu-id="d7a59-116">Methods</span></span>

| <span data-ttu-id="d7a59-117">Método</span><span class="sxs-lookup"><span data-stu-id="d7a59-117">Method</span></span>       | <span data-ttu-id="d7a59-118">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d7a59-118">Return Type</span></span>  |<span data-ttu-id="d7a59-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7a59-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d7a59-120">Criar trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="d7a59-120">Create trustFrameworkPolicy</span></span>](../api/trustframework-post-trustframeworkpolicy.md)|<span data-ttu-id="d7a59-121">trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="d7a59-121">trustFrameworkPolicy</span></span>|<span data-ttu-id="d7a59-122">Criar um novo trustFrameworkPolicy.</span><span class="sxs-lookup"><span data-stu-id="d7a59-122">Create a new trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="d7a59-123">Obter trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="d7a59-123">Get trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-get.md) |<span data-ttu-id="d7a59-124">trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="d7a59-124">trustFrameworkPolicy</span></span>|<span data-ttu-id="d7a59-125">Ler as propriedades de um trustFrameworkPolicy existente.</span><span class="sxs-lookup"><span data-stu-id="d7a59-125">Read properties of an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="d7a59-126">Listar trustFrameworkPolicies</span><span class="sxs-lookup"><span data-stu-id="d7a59-126">List trustFrameworkPolicies</span></span>](../api/trustframework-list-trustframeworkpolicies.md)|<span data-ttu-id="d7a59-127">coleção trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="d7a59-127">trustFrameworkPolicy collection</span></span>|<span data-ttu-id="d7a59-128">Listar todos os trustFrameworkPolicies configurados em um locatário.</span><span class="sxs-lookup"><span data-stu-id="d7a59-128">List all trustFrameworkPolicies configured in a tenant.</span></span>|
|[<span data-ttu-id="d7a59-129">Atualizar ou criar trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="d7a59-129">Update or create trustFrameworkPolicy</span></span>](../api/trustframework-put-trustframeworkpolicy.md)|<span data-ttu-id="d7a59-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d7a59-130">None</span></span>|<span data-ttu-id="d7a59-131">Atualize um trustFrameworkPolicy existente.</span><span class="sxs-lookup"><span data-stu-id="d7a59-131">Update an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="d7a59-132">Excluir trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="d7a59-132">Delete trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-delete.md)|<span data-ttu-id="d7a59-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d7a59-133">None</span></span>|<span data-ttu-id="d7a59-134">Excluir um trustFrameworkPolicy existente.</span><span class="sxs-lookup"><span data-stu-id="d7a59-134">Delete an existing trustFrameworkPolicy.</span></span>|

## <a name="properties"></a><span data-ttu-id="d7a59-135">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d7a59-135">Properties</span></span>

|<span data-ttu-id="d7a59-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7a59-136">Property</span></span>|<span data-ttu-id="d7a59-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7a59-137">Type</span></span>|<span data-ttu-id="d7a59-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7a59-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7a59-139">id</span><span class="sxs-lookup"><span data-stu-id="d7a59-139">id</span></span>|<span data-ttu-id="d7a59-140">String</span><span class="sxs-lookup"><span data-stu-id="d7a59-140">String</span></span>|<span data-ttu-id="d7a59-141">A ID da política.</span><span class="sxs-lookup"><span data-stu-id="d7a59-141">The ID of the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7a59-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d7a59-142">JSON representation</span></span>

<span data-ttu-id="d7a59-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d7a59-143">The following is a JSON representation of the resource.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d7a59-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="d7a59-144">See also</span></span>

- <span data-ttu-id="d7a59-145">[trustFrameworkPolicy esquema](/azure/active-directory-b2c/trustframeworkpolicy) para obter informações sobre os elementos do esquema.</span><span class="sxs-lookup"><span data-stu-id="d7a59-145">[trustFrameworkPolicy schema](/azure/active-directory-b2c/trustframeworkpolicy) for information about the schema elements.</span></span>
- [<span data-ttu-id="d7a59-146">trustFrameworkPolicy. xsd</span><span class="sxs-lookup"><span data-stu-id="d7a59-146">trustFrameworkPolicy.xsd</span></span>](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)
