---
title: Tipo de recurso featureRolloutPolicy
description: Representa uma política de lançamento de recursos associada a um objeto de diretório.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: feed3844717dffbfcc98a0e11db31da4a0550e05
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945674"
---
# <a name="featurerolloutpolicy-resource-type"></a><span data-ttu-id="c13a6-103">Tipo de recurso featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c13a6-103">featureRolloutPolicy resource type</span></span>

<span data-ttu-id="c13a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c13a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c13a6-105">Representa uma política de lançamento de recursos associada a um objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="c13a6-105">Represents a feature rollout policy associated with a directory object.</span></span> <span data-ttu-id="c13a6-106">A criação de uma política de lançamento de recursos ajuda os administradores de locatários a criar recursos piloto do Azure AD com um grupo específico antes de habilenciar recursos para toda a organização.</span><span class="sxs-lookup"><span data-stu-id="c13a6-106">Creating a feature rollout policy helps tenant administrators to pilot features of Azure AD with a specific group before enabling features for entire organization.</span></span> <span data-ttu-id="c13a6-107">Isso minimiza o impacto e ajuda os administradores a testar e lançar gradualmente os recursos relacionados à autenticação.</span><span class="sxs-lookup"><span data-stu-id="c13a6-107">This minimizes the impact and helps administrators to test and rollout authentication related features gradually.</span></span>

<span data-ttu-id="c13a6-108">Veja a seguir as limitações da adoção de recursos:</span><span class="sxs-lookup"><span data-stu-id="c13a6-108">The following are limitations of feature rollout:</span></span>

- <span data-ttu-id="c13a6-109">Cada recurso oferece suporte a no máximo 10 grupos.</span><span class="sxs-lookup"><span data-stu-id="c13a6-109">Each feature supports a maximum of 10 groups.</span></span>
- <span data-ttu-id="c13a6-110">O **campo appliesTo só** dá suporte a grupos.</span><span class="sxs-lookup"><span data-stu-id="c13a6-110">The **appliesTo** field only supports groups.</span></span>
- <span data-ttu-id="c13a6-111">Não há suporte para grupos dinâmicos e grupos aninhados.</span><span class="sxs-lookup"><span data-stu-id="c13a6-111">Dynamic groups and nested groups are not supported.</span></span>

<span data-ttu-id="c13a6-112">A seguir estão os pré-requisitos para cada um dos recursos atualmente com suporte para a adoção usando essa política de lançamento.</span><span class="sxs-lookup"><span data-stu-id="c13a6-112">The following are pre-requisites for each of the features that are currently suported for rollout using this rollout policy.</span></span>

### <a name="passthrough-authentication"></a><span data-ttu-id="c13a6-113">Autenticação passo a passo</span><span class="sxs-lookup"><span data-stu-id="c13a6-113">Passthrough Authentication</span></span>

* <span data-ttu-id="c13a6-114">Identifique um servidor executando o Windows Server 2012 R2 ou posterior onde você deseja que o [Agente PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) seja executado.</span><span class="sxs-lookup"><span data-stu-id="c13a6-114">Identify a server running Windows Server 2012 R2 or later where you want the [PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) Agent to run.</span></span><span data-ttu-id="c13a6-115">Verifique se o servidor está ingressado no domínio, pode autenticar usuários selecionados com o Active Directory e pode se comunicar com o Azure AD em portas de saída/URLs.</span><span class="sxs-lookup"><span data-stu-id="c13a6-115"> Ensure that the server is domain-joined, can authenticate selected users with Active Directory, and can communicate with Azure AD on outbound ports / URLs.</span></span>
* <span data-ttu-id="c13a6-116">[Baixe](https://aka.ms/getauthagent) & instalar o Agente de Autenticação do Microsoft Azure AD Connect no servidor.</span><span class="sxs-lookup"><span data-stu-id="c13a6-116">[Download](https://aka.ms/getauthagent) & install the Microsoft Azure AD Connect Authentication Agent on the server.</span></span>
* <span data-ttu-id="c13a6-117">Para habilitar alta disponibilidade, instale agentes de autenticação adicionais em outros servidores conforme descrito [aqui](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span><span class="sxs-lookup"><span data-stu-id="c13a6-117">To enable high availability, install additional Authentication Agents on other servers as described [here](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span></span>
* <span data-ttu-id="c13a6-118">Verifique se você configurou suas [configurações de Bloqueio](/azure/active-directory/authentication/howto-password-smart-lockout) Inteligente adequadamente.</span><span class="sxs-lookup"><span data-stu-id="c13a6-118">Ensure that you have configured your [Smart Lockout](/azure/active-directory/authentication/howto-password-smart-lockout) settings appropriately.</span></span> <span data-ttu-id="c13a6-119">Isso é para garantir que as contas locais do Active Directory de seus usuários não são bloqueadas por atores ruins.</span><span class="sxs-lookup"><span data-stu-id="c13a6-119">This is to ensure that your users’ on-premises Active Directory accounts don’t get locked out by bad actors.</span></span>

### <a name="seamlesssso"></a><span data-ttu-id="c13a6-120">SeamlessSso</span><span class="sxs-lookup"><span data-stu-id="c13a6-120">SeamlessSso</span></span>

* <span data-ttu-id="c13a6-121">[Habilita o SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) para as florestas do AD com base [nessas](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) instruções.</span><span class="sxs-lookup"><span data-stu-id="c13a6-121">Enable [SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) for the AD forests based on [these](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) instructions.</span></span>

### <a name="passwordhashsync"></a><span data-ttu-id="c13a6-122">PasswordHashSync</span><span class="sxs-lookup"><span data-stu-id="c13a6-122">PasswordHashSync</span></span>

* <span data-ttu-id="c13a6-123"> [Habilitar PasswordHashSync](/azure/active-directory/hybrid/whatis-phs)na página   "Recursos opcionais" no Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="c13a6-123">Enable [PasswordHashSync](/azure/active-directory/hybrid/whatis-phs) from the “Optional features” page in Azure AD Connect.</span></span>

### <a name="emailasalternateid"></a><span data-ttu-id="c13a6-124">EmailAsAlternateId</span><span class="sxs-lookup"><span data-stu-id="c13a6-124">EmailAsAlternateId</span></span>

* <span data-ttu-id="c13a6-125">Associe emails alternativos a contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="c13a6-125">Associate alternate email  with user accounts.</span></span>

## <a name="methods"></a><span data-ttu-id="c13a6-126">Métodos</span><span class="sxs-lookup"><span data-stu-id="c13a6-126">Methods</span></span>

| <span data-ttu-id="c13a6-127">Método</span><span class="sxs-lookup"><span data-stu-id="c13a6-127">Method</span></span>                                                                         | <span data-ttu-id="c13a6-128">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c13a6-128">Return Type</span></span>                                     | <span data-ttu-id="c13a6-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="c13a6-129">Description</span></span>                                                               |
|:-------------------------------------------------------------------------------|:------------------------------------------------|:--------------------------------------------------------------------------|
| [<span data-ttu-id="c13a6-130">Listar featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="c13a6-130">List featureRolloutPolicies</span></span>](../api/list-featurerolloutpolicies.md) | [<span data-ttu-id="c13a6-131">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c13a6-131">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="c13a6-132">Recupere uma lista de objetos featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="c13a6-132">Retrieve a list of featureRolloutPolicy objects.</span></span>                          |
| [<span data-ttu-id="c13a6-133">Obter featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c13a6-133">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md)                 | [<span data-ttu-id="c13a6-134">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c13a6-134">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="c13a6-135">Recupere as propriedades e as relações do objeto featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="c13a6-135">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="c13a6-136">Criar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c13a6-136">Create featureRolloutPolicy</span></span>](../api/post-featurerolloutpolicies.md) | [<span data-ttu-id="c13a6-137">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c13a6-137">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="c13a6-138">Crie um novo objeto featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="c13a6-138">Create a new featureRolloutPolicy object.</span></span>                                 |
| [<span data-ttu-id="c13a6-139">Atualizar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c13a6-139">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md)           | [<span data-ttu-id="c13a6-140">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c13a6-140">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="c13a6-141">Atualize as propriedades do objeto featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="c13a6-141">Update the properties of featurerolloutpolicy object.</span></span>                     |
| [<span data-ttu-id="c13a6-142">Excluir featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c13a6-142">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md)           | <span data-ttu-id="c13a6-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c13a6-143">None</span></span>                                            | <span data-ttu-id="c13a6-144">Exclua um objeto featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="c13a6-144">Delete a featureRolloutPolicy object.</span></span>                                     |
| [<span data-ttu-id="c13a6-145">Atribuir appliesTo</span><span class="sxs-lookup"><span data-stu-id="c13a6-145">Assign appliesTo</span></span>](../api/featurerolloutpolicy-post-appliesto.md)              | [<span data-ttu-id="c13a6-146">directoryObject</span><span class="sxs-lookup"><span data-stu-id="c13a6-146">directoryObject</span></span>](directoryobject.md)           | <span data-ttu-id="c13a6-147">Atribua um directoryObject à atribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="c13a6-147">Assign a directoryObject to feature rollout.</span></span>                              |
| [<span data-ttu-id="c13a6-148">Remover appliesTo</span><span class="sxs-lookup"><span data-stu-id="c13a6-148">Remove appliesTo</span></span>](../api/featurerolloutpolicy-delete-appliesto.md)            | <span data-ttu-id="c13a6-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c13a6-149">None</span></span>                                            | <span data-ttu-id="c13a6-150">Remover um directoryObject da adoção de recursos.</span><span class="sxs-lookup"><span data-stu-id="c13a6-150">Remove a directoryObject from feature rollout.</span></span>                            |

## <a name="properties"></a><span data-ttu-id="c13a6-151">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c13a6-151">Properties</span></span>

| <span data-ttu-id="c13a6-152">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c13a6-152">Property</span></span>     | <span data-ttu-id="c13a6-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="c13a6-153">Type</span></span>        | <span data-ttu-id="c13a6-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="c13a6-154">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c13a6-155">description</span><span class="sxs-lookup"><span data-stu-id="c13a6-155">description</span></span>|<span data-ttu-id="c13a6-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c13a6-156">String</span></span>|<span data-ttu-id="c13a6-157">Uma descrição para essa política de lançamento de recursos.</span><span class="sxs-lookup"><span data-stu-id="c13a6-157">A description for this feature rollout policy.</span></span>|
|<span data-ttu-id="c13a6-158">displayName</span><span class="sxs-lookup"><span data-stu-id="c13a6-158">displayName</span></span>|<span data-ttu-id="c13a6-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c13a6-159">String</span></span>|<span data-ttu-id="c13a6-160">O nome de exibição dessa política de lançamento de recursos.</span><span class="sxs-lookup"><span data-stu-id="c13a6-160">The display name for this  feature rollout policy.</span></span>|
|<span data-ttu-id="c13a6-161">feature</span><span class="sxs-lookup"><span data-stu-id="c13a6-161">feature</span></span>|<span data-ttu-id="c13a6-162">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="c13a6-162">stagedFeatureName</span></span>| <span data-ttu-id="c13a6-163">Os valores possíveis são: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `emailAsAlternateId`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c13a6-163">Possible values are: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `emailAsAlternateId`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c13a6-164">id</span><span class="sxs-lookup"><span data-stu-id="c13a6-164">id</span></span>|<span data-ttu-id="c13a6-165">String</span><span class="sxs-lookup"><span data-stu-id="c13a6-165">String</span></span>| <span data-ttu-id="c13a6-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c13a6-166">Read-only.</span></span>|
|<span data-ttu-id="c13a6-167">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="c13a6-167">isAppliedToOrganization</span></span>|<span data-ttu-id="c13a6-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="c13a6-168">Boolean</span></span>|<span data-ttu-id="c13a6-169">Indica se essa política de lançamento de recursos deve ser aplicada a toda a organização.</span><span class="sxs-lookup"><span data-stu-id="c13a6-169">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="c13a6-170">isEnabled</span><span class="sxs-lookup"><span data-stu-id="c13a6-170">isEnabled</span></span>|<span data-ttu-id="c13a6-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="c13a6-171">Boolean</span></span>|<span data-ttu-id="c13a6-172">Indica se a adoção de recursos está habilitada.</span><span class="sxs-lookup"><span data-stu-id="c13a6-172">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c13a6-173">Relações</span><span class="sxs-lookup"><span data-stu-id="c13a6-173">Relationships</span></span>

| <span data-ttu-id="c13a6-174">Relação</span><span class="sxs-lookup"><span data-stu-id="c13a6-174">Relationship</span></span> | <span data-ttu-id="c13a6-175">Tipo</span><span class="sxs-lookup"><span data-stu-id="c13a6-175">Type</span></span>        | <span data-ttu-id="c13a6-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="c13a6-176">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c13a6-177">appliesTo</span><span class="sxs-lookup"><span data-stu-id="c13a6-177">appliesTo</span></span>|<span data-ttu-id="c13a6-178">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="c13a6-178">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="c13a6-179">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c13a6-179">Nullable.</span></span> <span data-ttu-id="c13a6-180">Especifica uma lista de directoryObjects para os qual o recurso está habilitado.</span><span class="sxs-lookup"><span data-stu-id="c13a6-180">Specifies a list of directoryObjects that feature is enabled for.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c13a6-181">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c13a6-181">JSON representation</span></span>

<span data-ttu-id="c13a6-182">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c13a6-182">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
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


