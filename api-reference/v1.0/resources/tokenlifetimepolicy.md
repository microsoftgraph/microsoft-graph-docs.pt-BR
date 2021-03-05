---
title: Tipo de recurso tokenLifetimePolicy
description: Representa uma política que pode controlar o tempo de vida de um token de acesso emitido pelo Azure Active Directory.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f950ce0c5a269aee5159349c76e9bea1c4c7a505
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442499"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="dd9f0-103">Tipo de recurso tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dd9f0-103">tokenLifetimePolicy resource type</span></span>

<span data-ttu-id="dd9f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd9f0-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="dd9f0-105">Representa uma política que pode controlar o tempo de vida de um token de acesso JWT, um token de ID ou um token SAML 1.1/2.0 emitido pelo Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="dd9f0-105">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="dd9f0-106">É possível definir tempos de vida do token para todos os aplicativos em sua organização, para um aplicativo multilocatário (organização múltipla) ou para uma entidade de serviço específica em sua organização.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-106">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span>  <span data-ttu-id="dd9f0-107">Para obter mais detalhes do cenário, [consulte Tempo de vida útil do token configurável no Azure Active Directory](/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="dd9f0-107">For more scenario details see [Configurable token lifetimes in Azure Active Directory](/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

><span data-ttu-id="dd9f0-108">**Observação:** Não há suporte para configurar essa política para Tokens de Atualização e Tokens de Sessão.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-108">**Note:** Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="dd9f0-109">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd9f0-109">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dd9f0-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="dd9f0-110">Methods</span></span>

| <span data-ttu-id="dd9f0-111">Método</span><span class="sxs-lookup"><span data-stu-id="dd9f0-111">Method</span></span>       | <span data-ttu-id="dd9f0-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dd9f0-112">Return Type</span></span> | <span data-ttu-id="dd9f0-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd9f0-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="dd9f0-114">Listar tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="dd9f0-114">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="dd9f0-115">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dd9f0-115">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="dd9f0-116">Leia propriedades e relações de objetos tokenLifetimePolicies.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-116">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="dd9f0-117">Criar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dd9f0-117">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="dd9f0-118">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dd9f0-118">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="dd9f0-119">Crie um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-119">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="dd9f0-120">Obter tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dd9f0-120">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="dd9f0-121">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dd9f0-121">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="dd9f0-122">Ler propriedades e relações de um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-122">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="dd9f0-123">Atualizar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dd9f0-123">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="dd9f0-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd9f0-124">None</span></span> | <span data-ttu-id="dd9f0-125">Atualize um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-125">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="dd9f0-126">Excluir tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dd9f0-126">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="dd9f0-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd9f0-127">None</span></span> | <span data-ttu-id="dd9f0-128">Exclua um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-128">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="dd9f0-129">Lista appliesTo</span><span class="sxs-lookup"><span data-stu-id="dd9f0-129">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="dd9f0-130">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="dd9f0-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="dd9f0-131">Obter a lista de directoryObjects aos qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-131">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="dd9f0-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd9f0-132">Properties</span></span>

| <span data-ttu-id="dd9f0-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd9f0-133">Property</span></span>     | <span data-ttu-id="dd9f0-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd9f0-134">Type</span></span>        | <span data-ttu-id="dd9f0-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd9f0-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dd9f0-136">id</span><span class="sxs-lookup"><span data-stu-id="dd9f0-136">id</span></span>|<span data-ttu-id="dd9f0-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd9f0-137">String</span></span>| <span data-ttu-id="dd9f0-138">Identificador exclusivo dessa política.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-138">Unique identifier for this policy.</span></span> <span data-ttu-id="dd9f0-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-139">Read-only.</span></span>|
|<span data-ttu-id="dd9f0-140">definition</span><span class="sxs-lookup"><span data-stu-id="dd9f0-140">definition</span></span>|<span data-ttu-id="dd9f0-141">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd9f0-141">String collection</span></span>| <span data-ttu-id="dd9f0-142">Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-142">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="dd9f0-143">Consulte abaixo para obter mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-143">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="dd9f0-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-144">Required.</span></span>|
|<span data-ttu-id="dd9f0-145">description</span><span class="sxs-lookup"><span data-stu-id="dd9f0-145">description</span></span>|<span data-ttu-id="dd9f0-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd9f0-146">String</span></span>| <span data-ttu-id="dd9f0-147">Descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-147">Description for this policy.</span></span>|
|<span data-ttu-id="dd9f0-148">displayName</span><span class="sxs-lookup"><span data-stu-id="dd9f0-148">displayName</span></span>|<span data-ttu-id="dd9f0-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd9f0-149">String</span></span>| <span data-ttu-id="dd9f0-150">Nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-150">Display name for this policy.</span></span> <span data-ttu-id="dd9f0-151">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-151">Required.</span></span>|
|<span data-ttu-id="dd9f0-152">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="dd9f0-152">isOrganizationDefault</span></span>|<span data-ttu-id="dd9f0-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd9f0-153">Boolean</span></span>|<span data-ttu-id="dd9f0-154">Se definido como true, ativa essa política.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-154">If set to true, activates this policy.</span></span> <span data-ttu-id="dd9f0-155">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como o padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-155">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="dd9f0-156">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-156">Optional, default value is false.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="dd9f0-157">Propriedades de uma definição de política de vida útil do token</span><span class="sxs-lookup"><span data-stu-id="dd9f0-157">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="dd9f0-158">As propriedades abaixo formam o objeto JSON que representa uma política de vida útil do token.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-158">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="dd9f0-159">Esse objeto JSON deve ser **convertido em uma cadeia de caracteres com** aspas que escapam para serem inseridas na propriedade **definition.**</span><span class="sxs-lookup"><span data-stu-id="dd9f0-159">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="dd9f0-160">Um exemplo é mostrado abaixo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="dd9f0-160">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="dd9f0-161">**Observação:** Todas as durações de tempo nessas propriedades são especificadas no formato "dd.hh:mm:ss".</span><span class="sxs-lookup"><span data-stu-id="dd9f0-161">**Note:** All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="dd9f0-162">**Observação:** Os valores máximos para propriedades anotadas em "dias" são 1 segundo a menos do número de dias anotado.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-162">**Note:** Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="dd9f0-163">Por exemplo, o valor máximo de 1 dia é especificado como "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="dd9f0-163">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="dd9f0-164">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd9f0-164">Property</span></span>     | <span data-ttu-id="dd9f0-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd9f0-165">Type</span></span>   |<span data-ttu-id="dd9f0-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd9f0-166">Description</span></span>| <span data-ttu-id="dd9f0-167">Valor Mínimo</span><span class="sxs-lookup"><span data-stu-id="dd9f0-167">Min Value</span></span> | <span data-ttu-id="dd9f0-168">Valor Máximo</span><span class="sxs-lookup"><span data-stu-id="dd9f0-168">Max Value</span></span> | <span data-ttu-id="dd9f0-169">Valor padrão</span><span class="sxs-lookup"><span data-stu-id="dd9f0-169">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="dd9f0-170">AccessTokenLifetime</span><span class="sxs-lookup"><span data-stu-id="dd9f0-170">AccessTokenLifetime</span></span>|<span data-ttu-id="dd9f0-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd9f0-171">String</span></span>|<span data-ttu-id="dd9f0-172">Controla por quanto tempo os tokens de acesso e ID são considerados válidos.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-172">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="dd9f0-173">10 minutos</span><span class="sxs-lookup"><span data-stu-id="dd9f0-173">10 minutes</span></span>|<span data-ttu-id="dd9f0-174">1 dia</span><span class="sxs-lookup"><span data-stu-id="dd9f0-174">1 day</span></span>|<span data-ttu-id="dd9f0-175">1 hora</span><span class="sxs-lookup"><span data-stu-id="dd9f0-175">1 hour</span></span>|
|<span data-ttu-id="dd9f0-176">Versão</span><span class="sxs-lookup"><span data-stu-id="dd9f0-176">Version</span></span>|<span data-ttu-id="dd9f0-177">Inteiro</span><span class="sxs-lookup"><span data-stu-id="dd9f0-177">Integer</span></span>|<span data-ttu-id="dd9f0-178">Definir o valor de 1.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-178">Set value of 1.</span></span> <span data-ttu-id="dd9f0-179">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-179">Required.</span></span>|<span data-ttu-id="dd9f0-180">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd9f0-180">None</span></span>|<span data-ttu-id="dd9f0-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd9f0-181">None</span></span>|<span data-ttu-id="dd9f0-182">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd9f0-182">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd9f0-183">Relações</span><span class="sxs-lookup"><span data-stu-id="dd9f0-183">Relationships</span></span>

| <span data-ttu-id="dd9f0-184">Relação</span><span class="sxs-lookup"><span data-stu-id="dd9f0-184">Relationship</span></span> | <span data-ttu-id="dd9f0-185">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd9f0-185">Type</span></span>        | <span data-ttu-id="dd9f0-186">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd9f0-186">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dd9f0-187">appliesTo</span><span class="sxs-lookup"><span data-stu-id="dd9f0-187">appliesTo</span></span>|<span data-ttu-id="dd9f0-188">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="dd9f0-188">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="dd9f0-189">A [coleção directoryObject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-189">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="dd9f0-190">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-190">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dd9f0-191">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd9f0-191">JSON representation</span></span>

<span data-ttu-id="dd9f0-192">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dd9f0-192">The following is a JSON representation of the resource.</span></span>

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
