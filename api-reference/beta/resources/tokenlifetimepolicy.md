---
title: Tipo de recurso tokenLifetimePolicy
description: Representa uma política que pode controlar o tempo de vida de um token de acesso emitido pelo Azure Active Directory.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bcfe06a8a42db4b0cfd5c8dab8da2b753e195f2c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155500"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="c043d-103">Tipo de recurso tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="c043d-103">tokenLifetimePolicy resource type</span></span>

<span data-ttu-id="c043d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c043d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c043d-105">Representa uma política que pode controlar o tempo de vida de um token de acesso JWT, um token de ID ou um token SAML 1.1/2.0 emitido pelo Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="c043d-105">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="c043d-106">É possível definir tempos de vida do token para todos os aplicativos em sua organização, para um aplicativo multilocatário (organização múltipla) ou para uma entidade de serviço específica em sua organização.</span><span class="sxs-lookup"><span data-stu-id="c043d-106">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span>  <span data-ttu-id="c043d-107">Para obter mais detalhes do cenário, [consulte Tempo de vida de token configurável no Azure Active Directory.](/azure/active-directory/develop/active-directory-configurable-token-lifetimes)</span><span class="sxs-lookup"><span data-stu-id="c043d-107">For more scenario details see [Configurable token lifetimes in Azure Active Directory](/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

><span data-ttu-id="c043d-108">Observação: a configuração dessa política para Tokens de Atualização e Tokens de Sessão não é suportada.</span><span class="sxs-lookup"><span data-stu-id="c043d-108">Note: Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="c043d-109">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c043d-109">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c043d-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="c043d-110">Methods</span></span>

| <span data-ttu-id="c043d-111">Método</span><span class="sxs-lookup"><span data-stu-id="c043d-111">Method</span></span>       | <span data-ttu-id="c043d-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c043d-112">Return Type</span></span> | <span data-ttu-id="c043d-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="c043d-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c043d-114">Criar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="c043d-114">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="c043d-115">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="c043d-115">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="c043d-116">Crie um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="c043d-116">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="c043d-117">Obter tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="c043d-117">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="c043d-118">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="c043d-118">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="c043d-119">Ler propriedades e relações de um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="c043d-119">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="c043d-120">Listar tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="c043d-120">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="c043d-121">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="c043d-121">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="c043d-122">Leia as propriedades e os relacionamentos dos objetos tokenLifetimePolicies.</span><span class="sxs-lookup"><span data-stu-id="c043d-122">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="c043d-123">Atualizar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="c043d-123">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="c043d-124">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="c043d-124">None</span></span> | <span data-ttu-id="c043d-125">Atualize um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="c043d-125">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="c043d-126">Excluir tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="c043d-126">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="c043d-127">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="c043d-127">None</span></span> | <span data-ttu-id="c043d-128">Exclua um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="c043d-128">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="c043d-129">Lista appliesTo</span><span class="sxs-lookup"><span data-stu-id="c043d-129">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="c043d-130">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="c043d-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="c043d-131">Obter a lista de directoryObjects aos qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="c043d-131">Get the list of directoryObjects that this policy has been applied to.</span></span> |
| [<span data-ttu-id="c043d-132">Atribiur tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="c043d-132">Assign tokenLifetimePolicy</span></span>](../api/application-post-tokenlifetimepolicies.md) | <span data-ttu-id="c043d-133">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="c043d-133">None</span></span> | <span data-ttu-id="c043d-134">Atribua um objeto tokenLifetimePolicy a [um aplicativo ou](application.md) objeto [servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="c043d-134">Assign a tokenLifetimePolicy object to an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="c043d-135">Listar tokenLifetimePolicy atribuído</span><span class="sxs-lookup"><span data-stu-id="c043d-135">List assigned tokenLifetimePolicy</span></span>](../api/application-list-tokenlifetimepolicies.md) | <span data-ttu-id="c043d-136">Conjunto [tokenLifetimePolicy](tokenlifetimepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c043d-136">[tokenLifetimePolicy](tokenlifetimepolicy.md) collection</span></span> | <span data-ttu-id="c043d-137">Listar os objetos tokenLifetimePolicy atribuídos a um [aplicativo ou](application.md) [objeto servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="c043d-137">List the tokenLifetimePolicy objects that are assigned to an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="c043d-138">Remover tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="c043d-138">Remove tokenLifetimePolicy</span></span>](../api/application-delete-tokenlifetimepolicies.md) | <span data-ttu-id="c043d-139">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="c043d-139">None</span></span> | <span data-ttu-id="c043d-140">Remova um objeto tokenLifetimePolicy de um [aplicativo ou](application.md) [objeto servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="c043d-140">Remove a tokenLifetimePolicy object from an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c043d-141">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c043d-141">Properties</span></span>

| <span data-ttu-id="c043d-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c043d-142">Property</span></span>     | <span data-ttu-id="c043d-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="c043d-143">Type</span></span>        | <span data-ttu-id="c043d-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="c043d-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c043d-145">id</span><span class="sxs-lookup"><span data-stu-id="c043d-145">id</span></span>|<span data-ttu-id="c043d-146">String</span><span class="sxs-lookup"><span data-stu-id="c043d-146">String</span></span>| <span data-ttu-id="c043d-147">Identificador exclusivo desta política.</span><span class="sxs-lookup"><span data-stu-id="c043d-147">Unique identifier for this policy.</span></span> <span data-ttu-id="c043d-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c043d-148">Read-only.</span></span>|
|<span data-ttu-id="c043d-149">definição</span><span class="sxs-lookup"><span data-stu-id="c043d-149">definition</span></span>|<span data-ttu-id="c043d-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c043d-150">String collection</span></span>| <span data-ttu-id="c043d-151">Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política.</span><span class="sxs-lookup"><span data-stu-id="c043d-151">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="c043d-152">Veja abaixo para obter mais detalhes sobre o esquema JSON para essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="c043d-152">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="c043d-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c043d-153">Required.</span></span>|
|<span data-ttu-id="c043d-154">description</span><span class="sxs-lookup"><span data-stu-id="c043d-154">description</span></span>|<span data-ttu-id="c043d-155">String</span><span class="sxs-lookup"><span data-stu-id="c043d-155">String</span></span>| <span data-ttu-id="c043d-156">Descrição desta política.</span><span class="sxs-lookup"><span data-stu-id="c043d-156">Description for this policy.</span></span>|
|<span data-ttu-id="c043d-157">displayName</span><span class="sxs-lookup"><span data-stu-id="c043d-157">displayName</span></span>|<span data-ttu-id="c043d-158">String</span><span class="sxs-lookup"><span data-stu-id="c043d-158">String</span></span>| <span data-ttu-id="c043d-159">Nome para exibição desta política.</span><span class="sxs-lookup"><span data-stu-id="c043d-159">Display name for this policy.</span></span> <span data-ttu-id="c043d-160">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c043d-160">Required.</span></span>|
|<span data-ttu-id="c043d-161">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="c043d-161">isOrganizationDefault</span></span>|<span data-ttu-id="c043d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c043d-162">Boolean</span></span>|<span data-ttu-id="c043d-163">Se definido como true, ativa essa política.</span><span class="sxs-lookup"><span data-stu-id="c043d-163">If set to true, activates this policy.</span></span> <span data-ttu-id="c043d-164">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="c043d-164">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="c043d-165">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="c043d-165">Optional, default value is false.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="c043d-166">Propriedades de uma definição de política de tempo de vida do token</span><span class="sxs-lookup"><span data-stu-id="c043d-166">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="c043d-167">As propriedades abaixo formam o objeto JSON que representa uma política de tempo de vida do token.</span><span class="sxs-lookup"><span data-stu-id="c043d-167">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="c043d-168">Esse objeto JSON deve ser **convertido em uma cadeia de caracteres** com aspas que não devem ser inseridas na propriedade de **definição.**</span><span class="sxs-lookup"><span data-stu-id="c043d-168">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="c043d-169">Um exemplo é mostrado abaixo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="c043d-169">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="c043d-170">Observação: todas as durações nessas propriedades são especificadas no formato "dd.hh:mm:ss".</span><span class="sxs-lookup"><span data-stu-id="c043d-170">Note: All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="c043d-171">Observação: os valores máximos para propriedades anotadas em "dias" são 1 segundo a menos do número de dias anotado.</span><span class="sxs-lookup"><span data-stu-id="c043d-171">Note: Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="c043d-172">Por exemplo, o valor máximo de 1 dia é especificado como "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="c043d-172">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="c043d-173">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c043d-173">Property</span></span>     | <span data-ttu-id="c043d-174">Tipo</span><span class="sxs-lookup"><span data-stu-id="c043d-174">Type</span></span>   |<span data-ttu-id="c043d-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="c043d-175">Description</span></span>| <span data-ttu-id="c043d-176">Valor Mínimo</span><span class="sxs-lookup"><span data-stu-id="c043d-176">Min Value</span></span> | <span data-ttu-id="c043d-177">Valor Máximo</span><span class="sxs-lookup"><span data-stu-id="c043d-177">Max Value</span></span> | <span data-ttu-id="c043d-178">Valor padrão</span><span class="sxs-lookup"><span data-stu-id="c043d-178">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="c043d-179">AccessTokenLifetime</span><span class="sxs-lookup"><span data-stu-id="c043d-179">AccessTokenLifetime</span></span>|<span data-ttu-id="c043d-180">String</span><span class="sxs-lookup"><span data-stu-id="c043d-180">String</span></span>|<span data-ttu-id="c043d-181">Controla por quanto tempo os tokens de acesso e de ID são considerados válidos.</span><span class="sxs-lookup"><span data-stu-id="c043d-181">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="c043d-182">10 minutos</span><span class="sxs-lookup"><span data-stu-id="c043d-182">10 minutes</span></span>|<span data-ttu-id="c043d-183">1 dia</span><span class="sxs-lookup"><span data-stu-id="c043d-183">1 day</span></span>|<span data-ttu-id="c043d-184">1 hora</span><span class="sxs-lookup"><span data-stu-id="c043d-184">1 hour</span></span>|
|<span data-ttu-id="c043d-185">Versão</span><span class="sxs-lookup"><span data-stu-id="c043d-185">Version</span></span>|<span data-ttu-id="c043d-186">Inteiro</span><span class="sxs-lookup"><span data-stu-id="c043d-186">Integer</span></span>|<span data-ttu-id="c043d-187">Valor definido de 1.</span><span class="sxs-lookup"><span data-stu-id="c043d-187">Set value of 1.</span></span> <span data-ttu-id="c043d-188">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c043d-188">Required.</span></span>|<span data-ttu-id="c043d-189">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c043d-189">None</span></span>|<span data-ttu-id="c043d-190">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c043d-190">None</span></span>|<span data-ttu-id="c043d-191">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c043d-191">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="c043d-192">Relações</span><span class="sxs-lookup"><span data-stu-id="c043d-192">Relationships</span></span>

| <span data-ttu-id="c043d-193">Relação</span><span class="sxs-lookup"><span data-stu-id="c043d-193">Relationship</span></span> | <span data-ttu-id="c043d-194">Tipo</span><span class="sxs-lookup"><span data-stu-id="c043d-194">Type</span></span>        | <span data-ttu-id="c043d-195">Descrição</span><span class="sxs-lookup"><span data-stu-id="c043d-195">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c043d-196">appliesTo</span><span class="sxs-lookup"><span data-stu-id="c043d-196">appliesTo</span></span>|<span data-ttu-id="c043d-197">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="c043d-197">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="c043d-198">A [coleção directoryObject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="c043d-198">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="c043d-199">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c043d-199">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c043d-200">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c043d-200">JSON representation</span></span>

<span data-ttu-id="c043d-201">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c043d-201">The following is a JSON representation of the resource.</span></span>

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