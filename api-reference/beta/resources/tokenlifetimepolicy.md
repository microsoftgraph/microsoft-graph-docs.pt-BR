---
title: tipo de recurso tokenLifetimePolicy
description: Representa uma política que pode controlar o tempo de vida de um token de acesso emitido pelo Azure Active Directory.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 143898e33e3e3474bd5caf0d7855ff19a15e4e13
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006965"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="9302e-103">tipo de recurso tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="9302e-103">tokenLifetimePolicy resource type</span></span>

<span data-ttu-id="9302e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9302e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9302e-105">Representa uma política que pode controlar o tempo de vida de um token de acesso JWT, um token de ID ou um token SAML 1.1/2.0 emitido pelo Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="9302e-105">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="9302e-106">Você pode definir vidas úteis de token para todos os aplicativos em sua organização, para um aplicativo multilocatário (várias organizações) ou para uma entidade de serviço específica em sua organização.</span><span class="sxs-lookup"><span data-stu-id="9302e-106">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span>  <span data-ttu-id="9302e-107">Para obter mais detalhes do cenário, consulte [tempos de vida de token configuráveis no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="9302e-107">For more scenario details see [Configurable token lifetimes in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

><span data-ttu-id="9302e-108">Observação: não há suporte para a configuração dessa política para tokens de atualização e de sessão.</span><span class="sxs-lookup"><span data-stu-id="9302e-108">Note: Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="9302e-109">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9302e-109">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9302e-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="9302e-110">Methods</span></span>

| <span data-ttu-id="9302e-111">Método</span><span class="sxs-lookup"><span data-stu-id="9302e-111">Method</span></span>       | <span data-ttu-id="9302e-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9302e-112">Return Type</span></span> | <span data-ttu-id="9302e-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="9302e-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9302e-114">Criar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="9302e-114">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="9302e-115">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="9302e-115">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="9302e-116">Criar um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="9302e-116">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="9302e-117">Obter tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="9302e-117">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="9302e-118">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="9302e-118">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="9302e-119">Ler propriedades e relações de um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="9302e-119">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="9302e-120">Listar tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="9302e-120">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="9302e-121">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="9302e-121">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="9302e-122">Ler propriedades e relações de objetos tokenLifetimePolicies.</span><span class="sxs-lookup"><span data-stu-id="9302e-122">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="9302e-123">Atualizar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="9302e-123">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="9302e-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9302e-124">None</span></span> | <span data-ttu-id="9302e-125">Atualizar um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="9302e-125">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="9302e-126">Excluir tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="9302e-126">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="9302e-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9302e-127">None</span></span> | <span data-ttu-id="9302e-128">Excluir um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="9302e-128">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="9302e-129">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="9302e-129">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="9302e-130">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="9302e-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="9302e-131">Obtenha a lista de directoryObjects à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="9302e-131">Get the list of directoryObjects that this policy has been applied to.</span></span> |
| [<span data-ttu-id="9302e-132">Atribiur tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="9302e-132">Assign tokenLifetimePolicy</span></span>](../api/application-post-tokenlifetimepolicies.md) | <span data-ttu-id="9302e-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9302e-133">None</span></span> | <span data-ttu-id="9302e-134">Atribuir um objeto tokenLifetimePolicy a um objeto [Application](application.md) ou [servicePrincipalName](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="9302e-134">Assign a tokenLifetimePolicy object to an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="9302e-135">Lista atribuída tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="9302e-135">List assigned tokenLifetimePolicy</span></span>](../api/application-list-tokenlifetimepolicies.md) | <span data-ttu-id="9302e-136">Coleção [tokenLifetimePolicy](tokenlifetimepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9302e-136">[tokenLifetimePolicy](tokenlifetimepolicy.md) collection</span></span> | <span data-ttu-id="9302e-137">Lista os objetos tokenLifetimePolicy que são atribuídos a um objeto [Application](application.md) ou [servicePrincipalName](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="9302e-137">List the tokenLifetimePolicy objects that are assigned to an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="9302e-138">Remover tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="9302e-138">Remove tokenLifetimePolicy</span></span>](../api/application-delete-tokenlifetimepolicies.md) | <span data-ttu-id="9302e-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9302e-139">None</span></span> | <span data-ttu-id="9302e-140">Remover um objeto tokenLifetimePolicy de um objeto [Application](application.md) ou [servicePrincipalName](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="9302e-140">Remove a tokenLifetimePolicy object from an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9302e-141">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9302e-141">Properties</span></span>

| <span data-ttu-id="9302e-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9302e-142">Property</span></span>     | <span data-ttu-id="9302e-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="9302e-143">Type</span></span>        | <span data-ttu-id="9302e-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="9302e-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9302e-145">id</span><span class="sxs-lookup"><span data-stu-id="9302e-145">id</span></span>|<span data-ttu-id="9302e-146">String</span><span class="sxs-lookup"><span data-stu-id="9302e-146">String</span></span>| <span data-ttu-id="9302e-147">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="9302e-147">Unique identifier for this policy.</span></span> <span data-ttu-id="9302e-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9302e-148">Read-only.</span></span>|
|<span data-ttu-id="9302e-149">definir</span><span class="sxs-lookup"><span data-stu-id="9302e-149">definition</span></span>|<span data-ttu-id="9302e-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9302e-150">String collection</span></span>| <span data-ttu-id="9302e-151">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="9302e-151">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="9302e-152">Veja mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="9302e-152">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="9302e-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9302e-153">Required.</span></span>|
|<span data-ttu-id="9302e-154">description</span><span class="sxs-lookup"><span data-stu-id="9302e-154">description</span></span>|<span data-ttu-id="9302e-155">String</span><span class="sxs-lookup"><span data-stu-id="9302e-155">String</span></span>| <span data-ttu-id="9302e-156">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="9302e-156">Description for this policy.</span></span>|
|<span data-ttu-id="9302e-157">displayName</span><span class="sxs-lookup"><span data-stu-id="9302e-157">displayName</span></span>|<span data-ttu-id="9302e-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9302e-158">String</span></span>| <span data-ttu-id="9302e-159">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="9302e-159">Display name for this policy.</span></span> <span data-ttu-id="9302e-160">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9302e-160">Required.</span></span>|
|<span data-ttu-id="9302e-161">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="9302e-161">isOrganizationDefault</span></span>|<span data-ttu-id="9302e-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="9302e-162">Boolean</span></span>|<span data-ttu-id="9302e-163">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="9302e-163">If set to true, activates this policy.</span></span> <span data-ttu-id="9302e-164">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="9302e-164">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="9302e-165">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="9302e-165">Optional, default value is false.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="9302e-166">Propriedades de uma definição de política de tempo de vida do token</span><span class="sxs-lookup"><span data-stu-id="9302e-166">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="9302e-167">As propriedades abaixo formam o objeto JSON que representa uma política de tempo de vida do token.</span><span class="sxs-lookup"><span data-stu-id="9302e-167">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="9302e-168">Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** .</span><span class="sxs-lookup"><span data-stu-id="9302e-168">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="9302e-169">Um exemplo é mostrado abaixo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="9302e-169">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="9302e-170">Observação: todas as durações de tempo nessas propriedades são especificadas no formato "dd. hh: mm: SS".</span><span class="sxs-lookup"><span data-stu-id="9302e-170">Note: All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="9302e-171">Observação: os valores máximos para propriedades denotadas em "dias" são 1 segundo curto do número de dias indicado.</span><span class="sxs-lookup"><span data-stu-id="9302e-171">Note: Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="9302e-172">Por exemplo, o valor máximo de 1 dia é especificado como "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="9302e-172">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="9302e-173">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9302e-173">Property</span></span>     | <span data-ttu-id="9302e-174">Tipo</span><span class="sxs-lookup"><span data-stu-id="9302e-174">Type</span></span>   |<span data-ttu-id="9302e-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="9302e-175">Description</span></span>| <span data-ttu-id="9302e-176">Valor mínimo</span><span class="sxs-lookup"><span data-stu-id="9302e-176">Min Value</span></span> | <span data-ttu-id="9302e-177">Valor máximo</span><span class="sxs-lookup"><span data-stu-id="9302e-177">Max Value</span></span> | <span data-ttu-id="9302e-178">Valor padrão</span><span class="sxs-lookup"><span data-stu-id="9302e-178">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="9302e-179">AccessTokenLifetime</span><span class="sxs-lookup"><span data-stu-id="9302e-179">AccessTokenLifetime</span></span>|<span data-ttu-id="9302e-180">String</span><span class="sxs-lookup"><span data-stu-id="9302e-180">String</span></span>|<span data-ttu-id="9302e-181">Controla por quanto tempo os tokens de acesso e de ID são considerados válidos.</span><span class="sxs-lookup"><span data-stu-id="9302e-181">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="9302e-182">10 minutos</span><span class="sxs-lookup"><span data-stu-id="9302e-182">10 minutes</span></span>|<span data-ttu-id="9302e-183">1 dia</span><span class="sxs-lookup"><span data-stu-id="9302e-183">1 day</span></span>|<span data-ttu-id="9302e-184">1 hora</span><span class="sxs-lookup"><span data-stu-id="9302e-184">1 hour</span></span>|
|<span data-ttu-id="9302e-185">Versão</span><span class="sxs-lookup"><span data-stu-id="9302e-185">Version</span></span>|<span data-ttu-id="9302e-186">Número inteiro</span><span class="sxs-lookup"><span data-stu-id="9302e-186">Integer</span></span>|<span data-ttu-id="9302e-187">Defina o valor 1.</span><span class="sxs-lookup"><span data-stu-id="9302e-187">Set value of 1.</span></span> <span data-ttu-id="9302e-188">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9302e-188">Required.</span></span>|<span data-ttu-id="9302e-189">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9302e-189">None</span></span>|<span data-ttu-id="9302e-190">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9302e-190">None</span></span>|<span data-ttu-id="9302e-191">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9302e-191">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="9302e-192">Relações</span><span class="sxs-lookup"><span data-stu-id="9302e-192">Relationships</span></span>

| <span data-ttu-id="9302e-193">Relação</span><span class="sxs-lookup"><span data-stu-id="9302e-193">Relationship</span></span> | <span data-ttu-id="9302e-194">Tipo</span><span class="sxs-lookup"><span data-stu-id="9302e-194">Type</span></span>        | <span data-ttu-id="9302e-195">Descrição</span><span class="sxs-lookup"><span data-stu-id="9302e-195">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9302e-196">appliesTo</span><span class="sxs-lookup"><span data-stu-id="9302e-196">appliesTo</span></span>|<span data-ttu-id="9302e-197">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="9302e-197">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="9302e-198">A coleção [directoryobject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="9302e-198">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="9302e-199">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9302e-199">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9302e-200">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9302e-200">JSON representation</span></span>

<span data-ttu-id="9302e-201">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9302e-201">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true,
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tokenLifetimePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->