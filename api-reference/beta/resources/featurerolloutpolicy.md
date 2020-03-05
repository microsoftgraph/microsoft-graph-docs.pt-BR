---
title: tipo de recurso featureRolloutPolicy
description: Representa uma política de distribuição de recursos associada a um objeto de diretório.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a5ebc5884b0fd1ccf52fca961247e610b1c8cad5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498480"
---
# <a name="featurerolloutpolicy-resource-type"></a><span data-ttu-id="fc773-103">tipo de recurso featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="fc773-103">featureRolloutPolicy resource type</span></span>

<span data-ttu-id="fc773-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fc773-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc773-105">Representa uma política de distribuição de recursos associada a um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="fc773-105">Represents a feature rollout policy associated with a directory object.</span></span> <span data-ttu-id="fc773-106">A criação de uma política de distribuição de recursos ajuda os administradores de locatários a recursos piloto do Azure AD com um grupo específico antes de habilitar recursos para toda a organização.</span><span class="sxs-lookup"><span data-stu-id="fc773-106">Creating a feature rollout policy helps tenant administrators to pilot features of Azure AD with a specific group before enabling features for entire organization.</span></span> <span data-ttu-id="fc773-107">Isso minimiza o impacto e ajuda os administradores a testar e a distribuir recursos relacionados à autenticação gradualmente.</span><span class="sxs-lookup"><span data-stu-id="fc773-107">This minimizes the impact and helps administrators to test and rollout authentication related features gradually.</span></span>

<span data-ttu-id="fc773-108">Veja a seguir as limitações da distribuição de recursos:</span><span class="sxs-lookup"><span data-stu-id="fc773-108">The following are limitations of feature rollout:</span></span>

- <span data-ttu-id="fc773-109">Cada recurso oferece suporte a um máximo de 10 grupos.</span><span class="sxs-lookup"><span data-stu-id="fc773-109">Each feature supports a maximum of 10 groups.</span></span>
- <span data-ttu-id="fc773-110">O campo **AppliesTo** só oferece suporte a grupos.</span><span class="sxs-lookup"><span data-stu-id="fc773-110">The **appliesTo** field only supports groups.</span></span>
- <span data-ttu-id="fc773-111">Não há suporte para grupos dinâmicos e aninhados.</span><span class="sxs-lookup"><span data-stu-id="fc773-111">Dynamic groups and nested groups are not supported.</span></span>

<span data-ttu-id="fc773-112">Estes são os requisitos para cada um dos recursos atualmente suported para distribuição usando esta política de distribuição.</span><span class="sxs-lookup"><span data-stu-id="fc773-112">The following are pre-requisites for each of the features that are currently suported for rollout using this rollout policy.</span></span>

### <a name="passthrough-authentication"></a><span data-ttu-id="fc773-113">Autenticação de passagem</span><span class="sxs-lookup"><span data-stu-id="fc773-113">Passthrough Authentication</span></span>

* <span data-ttu-id="fc773-114">Identifique um servidor executando o Windows Server 2012 R2 ou posterior onde você deseja que o agente do [PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) seja executado.</span><span class="sxs-lookup"><span data-stu-id="fc773-114">Identify a server running Windows Server 2012 R2 or later where you want the [PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) Agent to run.</span></span><span data-ttu-id="fc773-115">Certifique-se de que o servidor ingressou no domínio, possa autenticar usuários selecionados com o Active Directory e pode se comunicar com o Azure AD em portas/URLs de saída.</span><span class="sxs-lookup"><span data-stu-id="fc773-115"> Ensure that the server is domain-joined, can authenticate selected users with Active Directory, and can communicate with Azure AD on outbound ports / URLs.</span></span>
* <span data-ttu-id="fc773-116">[Baixe](https://aka.ms/getauthagent) & instale o agente de autenticação do Microsoft Azure ad Connect no servidor.</span><span class="sxs-lookup"><span data-stu-id="fc773-116">[Download](https://aka.ms/getauthagent) & install the Microsoft Azure AD Connect Authentication Agent on the server.</span></span>
* <span data-ttu-id="fc773-117">Para habilitar a alta disponibilidade, instale agentes de autenticação adicionais em outros servidores, conforme descrito [aqui](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span><span class="sxs-lookup"><span data-stu-id="fc773-117">To enable high availability, install additional Authentication Agents on other servers as described [here](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span></span>
* <span data-ttu-id="fc773-118">Verifique se você configurou suas configurações de [bloqueio inteligente](/azure/active-directory/authentication/howto-password-smart-lockout) adequadamente.</span><span class="sxs-lookup"><span data-stu-id="fc773-118">Ensure that you have configured your [Smart Lockout](/azure/active-directory/authentication/howto-password-smart-lockout) settings appropriately.</span></span> <span data-ttu-id="fc773-119">Isso é para garantir que as contas do Active Directory no local dos usuários não sejam bloqueadas por atores ruins.</span><span class="sxs-lookup"><span data-stu-id="fc773-119">This is to ensure that your users’ on-premises Active Directory accounts don’t get locked out by bad actors.</span></span>

### <a name="seamlesssso"></a><span data-ttu-id="fc773-120">SeamlessSso</span><span class="sxs-lookup"><span data-stu-id="fc773-120">SeamlessSso</span></span>

* <span data-ttu-id="fc773-121">Habilite o [SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) para as florestas do AD com [base nessas instruções.](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature)</span><span class="sxs-lookup"><span data-stu-id="fc773-121">Enable [SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) for the AD forests based on [these](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) instructions.</span></span>

### <a name="passwordhashsync"></a><span data-ttu-id="fc773-122">PasswordHashSync</span><span class="sxs-lookup"><span data-stu-id="fc773-122">PasswordHashSync</span></span>

* <span data-ttu-id="fc773-123">Habilite o [PasswordHashSync](/azure/active-directory/hybrid/whatis-phs) na página "recursos opcionais" no Azure ad Connect.</span><span class="sxs-lookup"><span data-stu-id="fc773-123">Enable [PasswordHashSync](/azure/active-directory/hybrid/whatis-phs) from the “Optional features” page in Azure AD Connect.</span></span>

## <a name="methods"></a><span data-ttu-id="fc773-124">Métodos</span><span class="sxs-lookup"><span data-stu-id="fc773-124">Methods</span></span>

| <span data-ttu-id="fc773-125">Método</span><span class="sxs-lookup"><span data-stu-id="fc773-125">Method</span></span>       | <span data-ttu-id="fc773-126">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fc773-126">Return Type</span></span> | <span data-ttu-id="fc773-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc773-127">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="fc773-128">Listar featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="fc773-128">List featureRolloutPolicies</span></span>](../api/directory-list-featurerolloutpolicies.md) | [<span data-ttu-id="fc773-129">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="fc773-129">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="fc773-130">Recupere uma lista de objetos featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="fc773-130">Retrieve a list of featureRolloutPolicy objects.</span></span> |
| [<span data-ttu-id="fc773-131">Obter featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="fc773-131">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md) | [<span data-ttu-id="fc773-132">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="fc773-132">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="fc773-133">Recupere as propriedades e os relacionamentos do objeto featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="fc773-133">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> ||
| [<span data-ttu-id="fc773-134">Criar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="fc773-134">Create featureRolloutPolicy</span></span>](../api/directory-post-featurerolloutpolicies.md) | [<span data-ttu-id="fc773-135">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="fc773-135">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="fc773-136">Criar um novo objeto featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="fc773-136">Create a new featureRolloutPolicy object.</span></span>
| [<span data-ttu-id="fc773-137">Atualizar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="fc773-137">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md) | [<span data-ttu-id="fc773-138">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="fc773-138">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="fc773-139">Atualize as propriedades do objeto featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="fc773-139">Update the properties of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="fc773-140">Excluir featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="fc773-140">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md) | <span data-ttu-id="fc773-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc773-141">None</span></span> | <span data-ttu-id="fc773-142">Excluir um objeto featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="fc773-142">Delete a featureRolloutPolicy object.</span></span> |
| [<span data-ttu-id="fc773-143">Atribuir aplica-se</span><span class="sxs-lookup"><span data-stu-id="fc773-143">Assign appliesTo</span></span>](../api/featurerolloutpolicy-post-appliesto.md) | [<span data-ttu-id="fc773-144">directoryObject</span><span class="sxs-lookup"><span data-stu-id="fc773-144">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="fc773-145">Atribua um directoryobject à distribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="fc773-145">Assign a directoryObject to feature rollout.</span></span> |
| [<span data-ttu-id="fc773-146">Remover aplica-se</span><span class="sxs-lookup"><span data-stu-id="fc773-146">Remove appliesTo</span></span>](../api/featurerolloutpolicy-delete-appliesto.md) | <span data-ttu-id="fc773-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc773-147">None</span></span> | <span data-ttu-id="fc773-148">Remover um directoryobject da distribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="fc773-148">Remove a directoryObject from feature rollout.</span></span> |

## <a name="properties"></a><span data-ttu-id="fc773-149">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc773-149">Properties</span></span>

| <span data-ttu-id="fc773-150">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc773-150">Property</span></span>     | <span data-ttu-id="fc773-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc773-151">Type</span></span>        | <span data-ttu-id="fc773-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc773-152">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fc773-153">description</span><span class="sxs-lookup"><span data-stu-id="fc773-153">description</span></span>|<span data-ttu-id="fc773-154">String</span><span class="sxs-lookup"><span data-stu-id="fc773-154">String</span></span>|<span data-ttu-id="fc773-155">Uma descrição para esta política de distribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="fc773-155">A description for this feature rollout policy.</span></span>|
|<span data-ttu-id="fc773-156">displayName</span><span class="sxs-lookup"><span data-stu-id="fc773-156">displayName</span></span>|<span data-ttu-id="fc773-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc773-157">String</span></span>|<span data-ttu-id="fc773-158">O nome de exibição desta política de distribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="fc773-158">The display name for this  feature rollout policy.</span></span>|
|<span data-ttu-id="fc773-159">apresentam</span><span class="sxs-lookup"><span data-stu-id="fc773-159">feature</span></span>|<span data-ttu-id="fc773-160">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="fc773-160">stagedFeatureName</span></span>| <span data-ttu-id="fc773-161">Os valores possíveis são: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="fc773-161">Possible values are: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="fc773-162">id</span><span class="sxs-lookup"><span data-stu-id="fc773-162">id</span></span>|<span data-ttu-id="fc773-163">String</span><span class="sxs-lookup"><span data-stu-id="fc773-163">String</span></span>| <span data-ttu-id="fc773-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fc773-164">Read-only.</span></span>|
|<span data-ttu-id="fc773-165">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="fc773-165">isAppliedToOrganization</span></span>|<span data-ttu-id="fc773-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc773-166">Boolean</span></span>|<span data-ttu-id="fc773-167">Indica se esta política de distribuição de recursos deve ser aplicada a toda a organização.</span><span class="sxs-lookup"><span data-stu-id="fc773-167">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="fc773-168">isEnabled</span><span class="sxs-lookup"><span data-stu-id="fc773-168">isEnabled</span></span>|<span data-ttu-id="fc773-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc773-169">Boolean</span></span>|<span data-ttu-id="fc773-170">Indica se a distribuição de recursos está habilitada.</span><span class="sxs-lookup"><span data-stu-id="fc773-170">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc773-171">Relações</span><span class="sxs-lookup"><span data-stu-id="fc773-171">Relationships</span></span>

| <span data-ttu-id="fc773-172">Relação</span><span class="sxs-lookup"><span data-stu-id="fc773-172">Relationship</span></span> | <span data-ttu-id="fc773-173">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc773-173">Type</span></span>        | <span data-ttu-id="fc773-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc773-174">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fc773-175">appliesTo</span><span class="sxs-lookup"><span data-stu-id="fc773-175">appliesTo</span></span>|<span data-ttu-id="fc773-176">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="fc773-176">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="fc773-177">Anulável.</span><span class="sxs-lookup"><span data-stu-id="fc773-177">Nullable.</span></span> <span data-ttu-id="fc773-178">Especifica uma lista de directoryObjects para o qual o recurso está habilitado.</span><span class="sxs-lookup"><span data-stu-id="fc773-178">Specifies a list of directoryObjects that feature is enabled for.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc773-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc773-179">JSON representation</span></span>

<span data-ttu-id="fc773-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc773-180">The following is a JSON representation of the resource.</span></span>

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
