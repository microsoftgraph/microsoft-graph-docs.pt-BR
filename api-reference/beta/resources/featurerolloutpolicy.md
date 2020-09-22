---
title: tipo de recurso featureRolloutPolicy
description: Representa uma política de distribuição de recursos associada a um objeto de diretório.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5c514d6a48ffafc13a118b9471fb94be9ffc0e11
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071203"
---
# <a name="featurerolloutpolicy-resource-type"></a><span data-ttu-id="23cc6-103">tipo de recurso featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="23cc6-103">featureRolloutPolicy resource type</span></span>

<span data-ttu-id="23cc6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23cc6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23cc6-105">Representa uma política de distribuição de recursos associada a um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="23cc6-105">Represents a feature rollout policy associated with a directory object.</span></span> <span data-ttu-id="23cc6-106">A criação de uma política de distribuição de recursos ajuda os administradores de locatários a recursos piloto do Azure AD com um grupo específico antes de habilitar recursos para toda a organização.</span><span class="sxs-lookup"><span data-stu-id="23cc6-106">Creating a feature rollout policy helps tenant administrators to pilot features of Azure AD with a specific group before enabling features for entire organization.</span></span> <span data-ttu-id="23cc6-107">Isso minimiza o impacto e ajuda os administradores a testar e a distribuir recursos relacionados à autenticação gradualmente.</span><span class="sxs-lookup"><span data-stu-id="23cc6-107">This minimizes the impact and helps administrators to test and rollout authentication related features gradually.</span></span>

<span data-ttu-id="23cc6-108">Veja a seguir as limitações da distribuição de recursos:</span><span class="sxs-lookup"><span data-stu-id="23cc6-108">The following are limitations of feature rollout:</span></span>

- <span data-ttu-id="23cc6-109">Cada recurso oferece suporte a um máximo de 10 grupos.</span><span class="sxs-lookup"><span data-stu-id="23cc6-109">Each feature supports a maximum of 10 groups.</span></span>
- <span data-ttu-id="23cc6-110">O campo **AppliesTo** só oferece suporte a grupos.</span><span class="sxs-lookup"><span data-stu-id="23cc6-110">The **appliesTo** field only supports groups.</span></span>
- <span data-ttu-id="23cc6-111">Não há suporte para grupos dinâmicos e aninhados.</span><span class="sxs-lookup"><span data-stu-id="23cc6-111">Dynamic groups and nested groups are not supported.</span></span>

<span data-ttu-id="23cc6-112">Estes são os requisitos para cada um dos recursos atualmente suported para distribuição usando esta política de distribuição.</span><span class="sxs-lookup"><span data-stu-id="23cc6-112">The following are pre-requisites for each of the features that are currently suported for rollout using this rollout policy.</span></span>

### <a name="passthrough-authentication"></a><span data-ttu-id="23cc6-113">Autenticação de passagem</span><span class="sxs-lookup"><span data-stu-id="23cc6-113">Passthrough Authentication</span></span>

* <span data-ttu-id="23cc6-114">Identifique um servidor executando o Windows Server 2012 R2 ou posterior onde você deseja que o agente do [PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) seja executado.</span><span class="sxs-lookup"><span data-stu-id="23cc6-114">Identify a server running Windows Server 2012 R2 or later where you want the [PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) Agent to run.</span></span><span data-ttu-id="23cc6-115">Certifique-se de que o servidor ingressou no domínio, possa autenticar usuários selecionados com o Active Directory e pode se comunicar com o Azure AD em portas/URLs de saída.</span><span class="sxs-lookup"><span data-stu-id="23cc6-115"> Ensure that the server is domain-joined, can authenticate selected users with Active Directory, and can communicate with Azure AD on outbound ports / URLs.</span></span>
* <span data-ttu-id="23cc6-116">[Baixe](https://aka.ms/getauthagent) & instale o agente de autenticação do Microsoft Azure ad Connect no servidor.</span><span class="sxs-lookup"><span data-stu-id="23cc6-116">[Download](https://aka.ms/getauthagent) & install the Microsoft Azure AD Connect Authentication Agent on the server.</span></span>
* <span data-ttu-id="23cc6-117">Para habilitar a alta disponibilidade, instale agentes de autenticação adicionais em outros servidores, conforme descrito [aqui](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span><span class="sxs-lookup"><span data-stu-id="23cc6-117">To enable high availability, install additional Authentication Agents on other servers as described [here](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span></span>
* <span data-ttu-id="23cc6-118">Verifique se você configurou suas configurações de [bloqueio inteligente](/azure/active-directory/authentication/howto-password-smart-lockout) adequadamente.</span><span class="sxs-lookup"><span data-stu-id="23cc6-118">Ensure that you have configured your [Smart Lockout](/azure/active-directory/authentication/howto-password-smart-lockout) settings appropriately.</span></span> <span data-ttu-id="23cc6-119">Isso é para garantir que as contas do Active Directory no local dos usuários não sejam bloqueadas por atores ruins.</span><span class="sxs-lookup"><span data-stu-id="23cc6-119">This is to ensure that your users’ on-premises Active Directory accounts don’t get locked out by bad actors.</span></span>

### <a name="seamlesssso"></a><span data-ttu-id="23cc6-120">SeamlessSso</span><span class="sxs-lookup"><span data-stu-id="23cc6-120">SeamlessSso</span></span>

* <span data-ttu-id="23cc6-121">Habilite o [SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) para as florestas do AD com [base nessas instruções.](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature)</span><span class="sxs-lookup"><span data-stu-id="23cc6-121">Enable [SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) for the AD forests based on [these](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) instructions.</span></span>

### <a name="passwordhashsync"></a><span data-ttu-id="23cc6-122">PasswordHashSync</span><span class="sxs-lookup"><span data-stu-id="23cc6-122">PasswordHashSync</span></span>

* <span data-ttu-id="23cc6-123">Habilite o [PasswordHashSync](/azure/active-directory/hybrid/whatis-phs)   na página "recursos opcionais" no Azure ad Connect.</span><span class="sxs-lookup"><span data-stu-id="23cc6-123">Enable [PasswordHashSync](/azure/active-directory/hybrid/whatis-phs) from the “Optional features” page in Azure AD Connect.</span></span>

### <a name="emailasalternateid"></a><span data-ttu-id="23cc6-124">EmailAsAlternateId</span><span class="sxs-lookup"><span data-stu-id="23cc6-124">EmailAsAlternateId</span></span>

* <span data-ttu-id="23cc6-125">Associe o email alternativo às contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="23cc6-125">Associate alternate email  with user accounts.</span></span>

## <a name="methods"></a><span data-ttu-id="23cc6-126">Métodos</span><span class="sxs-lookup"><span data-stu-id="23cc6-126">Methods</span></span>

| <span data-ttu-id="23cc6-127">Método</span><span class="sxs-lookup"><span data-stu-id="23cc6-127">Method</span></span>                                                                         | <span data-ttu-id="23cc6-128">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="23cc6-128">Return Type</span></span>                                     | <span data-ttu-id="23cc6-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="23cc6-129">Description</span></span>                                                               |
|:-------------------------------------------------------------------------------|:------------------------------------------------|:--------------------------------------------------------------------------|
| [<span data-ttu-id="23cc6-130">Listar featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="23cc6-130">List featureRolloutPolicies</span></span>](../api/directory-list-featurerolloutpolicies.md) | [<span data-ttu-id="23cc6-131">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="23cc6-131">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="23cc6-132">Recupere uma lista de objetos featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="23cc6-132">Retrieve a list of featureRolloutPolicy objects.</span></span>                          |
| [<span data-ttu-id="23cc6-133">Obter featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="23cc6-133">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md)                 | [<span data-ttu-id="23cc6-134">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="23cc6-134">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="23cc6-135">Recupere as propriedades e os relacionamentos do objeto featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="23cc6-135">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="23cc6-136">Criar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="23cc6-136">Create featureRolloutPolicy</span></span>](../api/directory-post-featurerolloutpolicies.md) | [<span data-ttu-id="23cc6-137">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="23cc6-137">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="23cc6-138">Criar um novo objeto featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="23cc6-138">Create a new featureRolloutPolicy object.</span></span>                                 |
| [<span data-ttu-id="23cc6-139">Atualizar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="23cc6-139">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md)           | [<span data-ttu-id="23cc6-140">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="23cc6-140">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="23cc6-141">Atualize as propriedades do objeto featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="23cc6-141">Update the properties of featurerolloutpolicy object.</span></span>                     |
| [<span data-ttu-id="23cc6-142">Excluir featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="23cc6-142">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md)           | <span data-ttu-id="23cc6-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23cc6-143">None</span></span>                                            | <span data-ttu-id="23cc6-144">Excluir um objeto featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="23cc6-144">Delete a featureRolloutPolicy object.</span></span>                                     |
| [<span data-ttu-id="23cc6-145">Atribuir aplica-se</span><span class="sxs-lookup"><span data-stu-id="23cc6-145">Assign appliesTo</span></span>](../api/featurerolloutpolicy-post-appliesto.md)              | [<span data-ttu-id="23cc6-146">directoryObject</span><span class="sxs-lookup"><span data-stu-id="23cc6-146">directoryObject</span></span>](directoryobject.md)           | <span data-ttu-id="23cc6-147">Atribua um directoryobject à distribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="23cc6-147">Assign a directoryObject to feature rollout.</span></span>                              |
| [<span data-ttu-id="23cc6-148">Remover aplica-se</span><span class="sxs-lookup"><span data-stu-id="23cc6-148">Remove appliesTo</span></span>](../api/featurerolloutpolicy-delete-appliesto.md)            | <span data-ttu-id="23cc6-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23cc6-149">None</span></span>                                            | <span data-ttu-id="23cc6-150">Remover um directoryobject da distribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="23cc6-150">Remove a directoryObject from feature rollout.</span></span>                            |

## <a name="properties"></a><span data-ttu-id="23cc6-151">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23cc6-151">Properties</span></span>

| <span data-ttu-id="23cc6-152">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23cc6-152">Property</span></span>     | <span data-ttu-id="23cc6-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="23cc6-153">Type</span></span>        | <span data-ttu-id="23cc6-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="23cc6-154">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="23cc6-155">description</span><span class="sxs-lookup"><span data-stu-id="23cc6-155">description</span></span>|<span data-ttu-id="23cc6-156">String</span><span class="sxs-lookup"><span data-stu-id="23cc6-156">String</span></span>|<span data-ttu-id="23cc6-157">Uma descrição para esta política de distribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="23cc6-157">A description for this feature rollout policy.</span></span>|
|<span data-ttu-id="23cc6-158">displayName</span><span class="sxs-lookup"><span data-stu-id="23cc6-158">displayName</span></span>|<span data-ttu-id="23cc6-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23cc6-159">String</span></span>|<span data-ttu-id="23cc6-160">O nome de exibição desta política de distribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="23cc6-160">The display name for this  feature rollout policy.</span></span>|
|<span data-ttu-id="23cc6-161">apresentam</span><span class="sxs-lookup"><span data-stu-id="23cc6-161">feature</span></span>|<span data-ttu-id="23cc6-162">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="23cc6-162">stagedFeatureName</span></span>| <span data-ttu-id="23cc6-163">Os valores possíveis são: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="23cc6-163">Possible values are: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="23cc6-164">id</span><span class="sxs-lookup"><span data-stu-id="23cc6-164">id</span></span>|<span data-ttu-id="23cc6-165">String</span><span class="sxs-lookup"><span data-stu-id="23cc6-165">String</span></span>| <span data-ttu-id="23cc6-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23cc6-166">Read-only.</span></span>|
|<span data-ttu-id="23cc6-167">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="23cc6-167">isAppliedToOrganization</span></span>|<span data-ttu-id="23cc6-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="23cc6-168">Boolean</span></span>|<span data-ttu-id="23cc6-169">Indica se esta política de distribuição de recursos deve ser aplicada a toda a organização.</span><span class="sxs-lookup"><span data-stu-id="23cc6-169">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="23cc6-170">isEnabled</span><span class="sxs-lookup"><span data-stu-id="23cc6-170">isEnabled</span></span>|<span data-ttu-id="23cc6-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="23cc6-171">Boolean</span></span>|<span data-ttu-id="23cc6-172">Indica se a distribuição de recursos está habilitada.</span><span class="sxs-lookup"><span data-stu-id="23cc6-172">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23cc6-173">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="23cc6-173">Relationships</span></span>

| <span data-ttu-id="23cc6-174">Relação</span><span class="sxs-lookup"><span data-stu-id="23cc6-174">Relationship</span></span> | <span data-ttu-id="23cc6-175">Tipo</span><span class="sxs-lookup"><span data-stu-id="23cc6-175">Type</span></span>        | <span data-ttu-id="23cc6-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="23cc6-176">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="23cc6-177">appliesTo</span><span class="sxs-lookup"><span data-stu-id="23cc6-177">appliesTo</span></span>|<span data-ttu-id="23cc6-178">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="23cc6-178">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="23cc6-179">Anulável.</span><span class="sxs-lookup"><span data-stu-id="23cc6-179">Nullable.</span></span> <span data-ttu-id="23cc6-180">Especifica uma lista de directoryObjects para o qual o recurso está habilitado.</span><span class="sxs-lookup"><span data-stu-id="23cc6-180">Specifies a list of directoryObjects that feature is enabled for.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="23cc6-181">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23cc6-181">JSON representation</span></span>

<span data-ttu-id="23cc6-182">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23cc6-182">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "feature": "string",
  "id": "String (identifier)",
  "isAppliedToOrganization": false,
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "featureRolloutPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


