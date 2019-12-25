---
title: tipo de recurso featureRolloutPolicy
description: Representa uma política de distribuição de recursos associada a um objeto de diretório.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 958e6750c9b6a0749613d3a380b43a7d1ab282c2
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870247"
---
# <a name="featurerolloutpolicy-resource-type"></a><span data-ttu-id="c3489-103">tipo de recurso featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c3489-103">featureRolloutPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3489-104">Representa uma política de distribuição de recursos associada a um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="c3489-104">Represents a feature rollout policy associated with a directory object.</span></span> <span data-ttu-id="c3489-105">A criação de uma política de distribuição de recursos ajuda os administradores de locatários a recursos piloto do Azure AD com um grupo específico antes de habilitar recursos para toda a organização.</span><span class="sxs-lookup"><span data-stu-id="c3489-105">Creating a feature rollout policy helps tenant administrators to pilot features of Azure AD with a specific group before enabling features for entire organization.</span></span> <span data-ttu-id="c3489-106">Isso minimiza o impacto e ajuda os administradores a testar e a distribuir recursos relacionados à autenticação gradualmente.</span><span class="sxs-lookup"><span data-stu-id="c3489-106">This minimizes the impact and helps administrators to test and rollout authentication related features gradually.</span></span>

<span data-ttu-id="c3489-107">Veja a seguir as limitações da distribuição de recursos:</span><span class="sxs-lookup"><span data-stu-id="c3489-107">The following are limitations of feature rollout:</span></span>

- <span data-ttu-id="c3489-108">Cada recurso oferece suporte a um máximo de 10 grupos.</span><span class="sxs-lookup"><span data-stu-id="c3489-108">Each feature supports a maximum of 10 groups.</span></span>
- <span data-ttu-id="c3489-109">O campo **AppliesTo** só oferece suporte a grupos.</span><span class="sxs-lookup"><span data-stu-id="c3489-109">The **appliesTo** field only supports groups.</span></span>
- <span data-ttu-id="c3489-110">Não há suporte para grupos dinâmicos e aninhados.</span><span class="sxs-lookup"><span data-stu-id="c3489-110">Dynamic groups and nested groups are not supported.</span></span>

<span data-ttu-id="c3489-111">Estes são os requisitos para cada um dos recursos atualmente suported para distribuição usando esta política de distribuição.</span><span class="sxs-lookup"><span data-stu-id="c3489-111">The following are pre-requisites for each of the features that are currently suported for rollout using this rollout policy.</span></span>

### <a name="passthrough-authentication"></a><span data-ttu-id="c3489-112">Autenticação de passagem</span><span class="sxs-lookup"><span data-stu-id="c3489-112">Passthrough Authentication</span></span>

* <span data-ttu-id="c3489-113">Identifique um servidor executando o Windows Server 2012 R2 ou posterior onde você deseja que o agente do [PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) seja executado.</span><span class="sxs-lookup"><span data-stu-id="c3489-113">Identify a server running Windows Server 2012 R2 or later where you want the [PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) Agent to run.</span></span><span data-ttu-id="c3489-114">Certifique-se de que o servidor ingressou no domínio, possa autenticar usuários selecionados com o Active Directory e pode se comunicar com o Azure AD em portas/URLs de saída.</span><span class="sxs-lookup"><span data-stu-id="c3489-114"> Ensure that the server is domain-joined, can authenticate selected users with Active Directory, and can communicate with Azure AD on outbound ports / URLs.</span></span>
* <span data-ttu-id="c3489-115">[Baixe](https://aka.ms/getauthagent) & instale o agente de autenticação do Microsoft Azure ad Connect no servidor.</span><span class="sxs-lookup"><span data-stu-id="c3489-115">[Download](https://aka.ms/getauthagent) & install the Microsoft Azure AD Connect Authentication Agent on the server.</span></span>
* <span data-ttu-id="c3489-116">Para habilitar a alta disponibilidade, instale agentes de autenticação adicionais em outros servidores, conforme descrito [aqui](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span><span class="sxs-lookup"><span data-stu-id="c3489-116">To enable high availability, install additional Authentication Agents on other servers as described [here](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span></span>
* <span data-ttu-id="c3489-117">Verifique se você configurou suas configurações de [bloqueio inteligente](/azure/active-directory/authentication/howto-password-smart-lockout) adequadamente.</span><span class="sxs-lookup"><span data-stu-id="c3489-117">Ensure that you have configured your [Smart Lockout](/azure/active-directory/authentication/howto-password-smart-lockout) settings appropriately.</span></span> <span data-ttu-id="c3489-118">Isso é para garantir que as contas do Active Directory no local dos usuários não sejam bloqueadas por atores ruins.</span><span class="sxs-lookup"><span data-stu-id="c3489-118">This is to ensure that your users’ on-premises Active Directory accounts don’t get locked out by bad actors.</span></span>

### <a name="seamlesssso"></a><span data-ttu-id="c3489-119">SeamlessSso</span><span class="sxs-lookup"><span data-stu-id="c3489-119">SeamlessSso</span></span>

* <span data-ttu-id="c3489-120">Habilite o [SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) para as florestas do AD com [base nessas instruções.](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature)</span><span class="sxs-lookup"><span data-stu-id="c3489-120">Enable [SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) for the AD forests based on [these](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) instructions.</span></span>

### <a name="passwordhashsync"></a><span data-ttu-id="c3489-121">PasswordHashSync</span><span class="sxs-lookup"><span data-stu-id="c3489-121">PasswordHashSync</span></span>

* <span data-ttu-id="c3489-122">Habilite o [PasswordHashSync](/azure/active-directory/hybrid/whatis-phs) na página "recursos opcionais" no Azure ad Connect.</span><span class="sxs-lookup"><span data-stu-id="c3489-122">Enable [PasswordHashSync](/azure/active-directory/hybrid/whatis-phs) from the “Optional features” page in Azure AD Connect.</span></span>

## <a name="methods"></a><span data-ttu-id="c3489-123">Métodos</span><span class="sxs-lookup"><span data-stu-id="c3489-123">Methods</span></span>

| <span data-ttu-id="c3489-124">Método</span><span class="sxs-lookup"><span data-stu-id="c3489-124">Method</span></span>       | <span data-ttu-id="c3489-125">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c3489-125">Return Type</span></span> | <span data-ttu-id="c3489-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3489-126">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c3489-127">Listar featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="c3489-127">List featureRolloutPolicies</span></span>](../api/directory-list-featurerolloutpolicies.md) | [<span data-ttu-id="c3489-128">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c3489-128">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="c3489-129">Recupere uma lista de objetos featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="c3489-129">Retrieve a list of featureRolloutPolicy objects.</span></span> |
| [<span data-ttu-id="c3489-130">Obter featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c3489-130">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md) | [<span data-ttu-id="c3489-131">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c3489-131">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="c3489-132">Recupere as propriedades e os relacionamentos do objeto featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="c3489-132">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> ||
| [<span data-ttu-id="c3489-133">Criar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c3489-133">Create featureRolloutPolicy</span></span>](../api/directory-post-featurerolloutpolicies.md) | [<span data-ttu-id="c3489-134">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c3489-134">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="c3489-135">Criar um novo objeto featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="c3489-135">Create a new featureRolloutPolicy object.</span></span>
| [<span data-ttu-id="c3489-136">Atualizar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c3489-136">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md) | [<span data-ttu-id="c3489-137">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c3489-137">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="c3489-138">Atualize as propriedades do objeto featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="c3489-138">Update the properties of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="c3489-139">Excluir featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c3489-139">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md) | <span data-ttu-id="c3489-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c3489-140">None</span></span> | <span data-ttu-id="c3489-141">Excluir um objeto featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="c3489-141">Delete a featureRolloutPolicy object.</span></span> |
| [<span data-ttu-id="c3489-142">Atribuir aplica-se</span><span class="sxs-lookup"><span data-stu-id="c3489-142">Assign appliesTo</span></span>](../api/featurerolloutpolicy-post-appliesto.md) | [<span data-ttu-id="c3489-143">directoryObject</span><span class="sxs-lookup"><span data-stu-id="c3489-143">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="c3489-144">Atribua um directoryobject à distribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="c3489-144">Assign a directoryObject to feature rollout.</span></span> |
| [<span data-ttu-id="c3489-145">Remover aplica-se</span><span class="sxs-lookup"><span data-stu-id="c3489-145">Remove appliesTo</span></span>](../api/featurerolloutpolicy-delete-appliesto.md) | <span data-ttu-id="c3489-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c3489-146">None</span></span> | <span data-ttu-id="c3489-147">Remover um directoryobject da distribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="c3489-147">Remove a directoryObject from feature rollout.</span></span> |

## <a name="properties"></a><span data-ttu-id="c3489-148">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3489-148">Properties</span></span>

| <span data-ttu-id="c3489-149">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3489-149">Property</span></span>     | <span data-ttu-id="c3489-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3489-150">Type</span></span>        | <span data-ttu-id="c3489-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3489-151">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c3489-152">description</span><span class="sxs-lookup"><span data-stu-id="c3489-152">description</span></span>|<span data-ttu-id="c3489-153">String</span><span class="sxs-lookup"><span data-stu-id="c3489-153">String</span></span>|<span data-ttu-id="c3489-154">Uma descrição para esta política de distribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="c3489-154">A description for this feature rollout policy.</span></span>|
|<span data-ttu-id="c3489-155">displayName</span><span class="sxs-lookup"><span data-stu-id="c3489-155">displayName</span></span>|<span data-ttu-id="c3489-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3489-156">String</span></span>|<span data-ttu-id="c3489-157">O nome de exibição desta política de distribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="c3489-157">The display name for this  feature rollout policy.</span></span>|
|<span data-ttu-id="c3489-158">apresentam</span><span class="sxs-lookup"><span data-stu-id="c3489-158">feature</span></span>|<span data-ttu-id="c3489-159">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="c3489-159">stagedFeatureName</span></span>| <span data-ttu-id="c3489-160">Os valores possíveis são: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c3489-160">Possible values are: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c3489-161">id</span><span class="sxs-lookup"><span data-stu-id="c3489-161">id</span></span>|<span data-ttu-id="c3489-162">String</span><span class="sxs-lookup"><span data-stu-id="c3489-162">String</span></span>| <span data-ttu-id="c3489-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3489-163">Read-only.</span></span>|
|<span data-ttu-id="c3489-164">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="c3489-164">isAppliedToOrganization</span></span>|<span data-ttu-id="c3489-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3489-165">Boolean</span></span>|<span data-ttu-id="c3489-166">Indica se esta política de distribuição de recursos deve ser aplicada a toda a organização.</span><span class="sxs-lookup"><span data-stu-id="c3489-166">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="c3489-167">isEnabled</span><span class="sxs-lookup"><span data-stu-id="c3489-167">isEnabled</span></span>|<span data-ttu-id="c3489-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3489-168">Boolean</span></span>|<span data-ttu-id="c3489-169">Indica se a distribuição de recursos está habilitada.</span><span class="sxs-lookup"><span data-stu-id="c3489-169">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3489-170">Relações</span><span class="sxs-lookup"><span data-stu-id="c3489-170">Relationships</span></span>

| <span data-ttu-id="c3489-171">Relação</span><span class="sxs-lookup"><span data-stu-id="c3489-171">Relationship</span></span> | <span data-ttu-id="c3489-172">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3489-172">Type</span></span>        | <span data-ttu-id="c3489-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3489-173">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c3489-174">appliesTo</span><span class="sxs-lookup"><span data-stu-id="c3489-174">appliesTo</span></span>|<span data-ttu-id="c3489-175">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="c3489-175">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="c3489-176">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c3489-176">Nullable.</span></span> <span data-ttu-id="c3489-177">Especifica uma lista de directoryObjects para o qual o recurso está habilitado.</span><span class="sxs-lookup"><span data-stu-id="c3489-177">Specifies a list of directoryObjects that feature is enabled for.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3489-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3489-178">JSON representation</span></span>

<span data-ttu-id="c3489-179">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3489-179">The following is a JSON representation of the resource.</span></span>

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
