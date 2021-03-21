---
title: Tipo de recurso tokenLifetimePolicy
description: Representa uma política que pode controlar o tempo de vida de um token de acesso emitido pelo Azure Active Directory.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: afc82ff81e9fd514cb95bd51ccb9df89e3577bd6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954964"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="e6ae3-103">Tipo de recurso tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e6ae3-103">tokenLifetimePolicy resource type</span></span>

<span data-ttu-id="e6ae3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6ae3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6ae3-105">Representa uma política que pode controlar o tempo de vida de um token de acesso JWT, um token de ID ou um token SAML 1.1/2.0 emitido pelo Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="e6ae3-105">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="e6ae3-106">É possível definir tempos de vida do token para todos os aplicativos em sua organização, para um aplicativo multilocatário (organização múltipla) ou para uma entidade de serviço específica em sua organização.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-106">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span>  <span data-ttu-id="e6ae3-107">Para obter mais detalhes do cenário, [consulte Tempo de vida útil do token configurável no Azure Active Directory](/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="e6ae3-107">For more scenario details see [Configurable token lifetimes in Azure Active Directory](/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

><span data-ttu-id="e6ae3-108">Observação: Não há suporte para configurar essa política para Tokens de Atualização e Tokens de Sessão.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-108">Note: Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="e6ae3-109">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e6ae3-109">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e6ae3-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="e6ae3-110">Methods</span></span>

| <span data-ttu-id="e6ae3-111">Método</span><span class="sxs-lookup"><span data-stu-id="e6ae3-111">Method</span></span>       | <span data-ttu-id="e6ae3-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e6ae3-112">Return Type</span></span> | <span data-ttu-id="e6ae3-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6ae3-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e6ae3-114">Criar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e6ae3-114">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="e6ae3-115">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e6ae3-115">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="e6ae3-116">Crie um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-116">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="e6ae3-117">Obter tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e6ae3-117">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="e6ae3-118">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e6ae3-118">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="e6ae3-119">Ler propriedades e relações de um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-119">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="e6ae3-120">Listar tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="e6ae3-120">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="e6ae3-121">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e6ae3-121">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="e6ae3-122">Leia propriedades e relações de objetos tokenLifetimePolicies.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-122">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="e6ae3-123">Atualizar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e6ae3-123">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="e6ae3-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6ae3-124">None</span></span> | <span data-ttu-id="e6ae3-125">Atualize um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-125">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="e6ae3-126">Excluir tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e6ae3-126">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="e6ae3-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6ae3-127">None</span></span> | <span data-ttu-id="e6ae3-128">Exclua um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-128">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="e6ae3-129">Lista appliesTo</span><span class="sxs-lookup"><span data-stu-id="e6ae3-129">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="e6ae3-130">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="e6ae3-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="e6ae3-131">Obter a lista de directoryObjects aos qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-131">Get the list of directoryObjects that this policy has been applied to.</span></span> |
| [<span data-ttu-id="e6ae3-132">Atribiur tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e6ae3-132">Assign tokenLifetimePolicy</span></span>](../api/application-post-tokenlifetimepolicies.md) | <span data-ttu-id="e6ae3-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6ae3-133">None</span></span> | <span data-ttu-id="e6ae3-134">Atribua um objeto tokenLifetimePolicy a [um aplicativo ou](application.md) objeto [servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="e6ae3-134">Assign a tokenLifetimePolicy object to an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="e6ae3-135">Listar token atribuídoLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e6ae3-135">List assigned tokenLifetimePolicy</span></span>](../api/application-list-tokenlifetimepolicies.md) | <span data-ttu-id="e6ae3-136">Conjunto [tokenLifetimePolicy](tokenlifetimepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e6ae3-136">[tokenLifetimePolicy](tokenlifetimepolicy.md) collection</span></span> | <span data-ttu-id="e6ae3-137">Listar os objetos tokenLifetimePolicy atribuídos a um [aplicativo](application.md) ou [objeto servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="e6ae3-137">List the tokenLifetimePolicy objects that are assigned to an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="e6ae3-138">Remover tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e6ae3-138">Remove tokenLifetimePolicy</span></span>](../api/application-delete-tokenlifetimepolicies.md) | <span data-ttu-id="e6ae3-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6ae3-139">None</span></span> | <span data-ttu-id="e6ae3-140">Remova um objeto tokenLifetimePolicy de [um aplicativo ou](application.md) objeto [servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="e6ae3-140">Remove a tokenLifetimePolicy object from an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e6ae3-141">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6ae3-141">Properties</span></span>

| <span data-ttu-id="e6ae3-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6ae3-142">Property</span></span>     | <span data-ttu-id="e6ae3-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6ae3-143">Type</span></span>        | <span data-ttu-id="e6ae3-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6ae3-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e6ae3-145">id</span><span class="sxs-lookup"><span data-stu-id="e6ae3-145">id</span></span>|<span data-ttu-id="e6ae3-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6ae3-146">String</span></span>| <span data-ttu-id="e6ae3-147">Identificador exclusivo dessa política.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-147">Unique identifier for this policy.</span></span> <span data-ttu-id="e6ae3-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-148">Read-only.</span></span>|
|<span data-ttu-id="e6ae3-149">definition</span><span class="sxs-lookup"><span data-stu-id="e6ae3-149">definition</span></span>|<span data-ttu-id="e6ae3-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6ae3-150">String collection</span></span>| <span data-ttu-id="e6ae3-151">Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-151">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="e6ae3-152">Consulte abaixo para obter mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-152">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="e6ae3-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-153">Required.</span></span>|
|<span data-ttu-id="e6ae3-154">description</span><span class="sxs-lookup"><span data-stu-id="e6ae3-154">description</span></span>|<span data-ttu-id="e6ae3-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6ae3-155">String</span></span>| <span data-ttu-id="e6ae3-156">Descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-156">Description for this policy.</span></span>|
|<span data-ttu-id="e6ae3-157">displayName</span><span class="sxs-lookup"><span data-stu-id="e6ae3-157">displayName</span></span>|<span data-ttu-id="e6ae3-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6ae3-158">String</span></span>| <span data-ttu-id="e6ae3-159">Nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-159">Display name for this policy.</span></span> <span data-ttu-id="e6ae3-160">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-160">Required.</span></span>|
|<span data-ttu-id="e6ae3-161">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="e6ae3-161">isOrganizationDefault</span></span>|<span data-ttu-id="e6ae3-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="e6ae3-162">Boolean</span></span>|<span data-ttu-id="e6ae3-163">Se definido como `true` , ativa essa política.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-163">If set to `true`, activates this policy.</span></span> <span data-ttu-id="e6ae3-164">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como o padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-164">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="e6ae3-165">Opcional, o valor padrão é `false` .</span><span class="sxs-lookup"><span data-stu-id="e6ae3-165">Optional, default value is `false`.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="e6ae3-166">Propriedades de uma definição de política de vida útil do token</span><span class="sxs-lookup"><span data-stu-id="e6ae3-166">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="e6ae3-167">As propriedades abaixo formam o objeto JSON que representa uma política de vida útil do token.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-167">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="e6ae3-168">Esse objeto JSON deve ser **convertido em uma cadeia de caracteres com** aspas que escapam para serem inseridas na propriedade **definition.**</span><span class="sxs-lookup"><span data-stu-id="e6ae3-168">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="e6ae3-169">Um exemplo é mostrado abaixo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="e6ae3-169">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="e6ae3-170">Observação: todas as durações de tempo nessas propriedades são especificadas no formato "dd.hh:mm:ss".</span><span class="sxs-lookup"><span data-stu-id="e6ae3-170">Note: All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="e6ae3-171">Observação: os valores máximos para propriedades anotadas em "dias" são 1 segundo a menos do número de dias anotado.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-171">Note: Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="e6ae3-172">Por exemplo, o valor máximo de 1 dia é especificado como "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="e6ae3-172">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="e6ae3-173">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6ae3-173">Property</span></span>     | <span data-ttu-id="e6ae3-174">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6ae3-174">Type</span></span>   |<span data-ttu-id="e6ae3-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6ae3-175">Description</span></span>| <span data-ttu-id="e6ae3-176">Valor Mínimo</span><span class="sxs-lookup"><span data-stu-id="e6ae3-176">Min Value</span></span> | <span data-ttu-id="e6ae3-177">Valor Máximo</span><span class="sxs-lookup"><span data-stu-id="e6ae3-177">Max Value</span></span> | <span data-ttu-id="e6ae3-178">Valor padrão</span><span class="sxs-lookup"><span data-stu-id="e6ae3-178">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="e6ae3-179">AccessTokenLifetime</span><span class="sxs-lookup"><span data-stu-id="e6ae3-179">AccessTokenLifetime</span></span>|<span data-ttu-id="e6ae3-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6ae3-180">String</span></span>|<span data-ttu-id="e6ae3-181">Controla por quanto tempo os tokens de acesso e ID são considerados válidos.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-181">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="e6ae3-182">10 minutos</span><span class="sxs-lookup"><span data-stu-id="e6ae3-182">10 minutes</span></span>|<span data-ttu-id="e6ae3-183">1 dia</span><span class="sxs-lookup"><span data-stu-id="e6ae3-183">1 day</span></span>|<span data-ttu-id="e6ae3-184">1 hora</span><span class="sxs-lookup"><span data-stu-id="e6ae3-184">1 hour</span></span>|
|<span data-ttu-id="e6ae3-185">Versão</span><span class="sxs-lookup"><span data-stu-id="e6ae3-185">Version</span></span>|<span data-ttu-id="e6ae3-186">Inteiro</span><span class="sxs-lookup"><span data-stu-id="e6ae3-186">Integer</span></span>|<span data-ttu-id="e6ae3-187">Definir o valor de 1.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-187">Set value of 1.</span></span> <span data-ttu-id="e6ae3-188">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-188">Required.</span></span>|<span data-ttu-id="e6ae3-189">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6ae3-189">None</span></span>|<span data-ttu-id="e6ae3-190">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6ae3-190">None</span></span>|<span data-ttu-id="e6ae3-191">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6ae3-191">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6ae3-192">Relações</span><span class="sxs-lookup"><span data-stu-id="e6ae3-192">Relationships</span></span>

| <span data-ttu-id="e6ae3-193">Relação</span><span class="sxs-lookup"><span data-stu-id="e6ae3-193">Relationship</span></span> | <span data-ttu-id="e6ae3-194">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6ae3-194">Type</span></span>        | <span data-ttu-id="e6ae3-195">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6ae3-195">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e6ae3-196">appliesTo</span><span class="sxs-lookup"><span data-stu-id="e6ae3-196">appliesTo</span></span>|<span data-ttu-id="e6ae3-197">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="e6ae3-197">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="e6ae3-198">A [coleção directoryObject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-198">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="e6ae3-199">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-199">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e6ae3-200">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6ae3-200">JSON representation</span></span>

<span data-ttu-id="e6ae3-201">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6ae3-201">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
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
