---
title: Tipo de recurso tokenLifetimePolicy
description: Representa uma política que pode controlar o tempo de vida de um token de acesso emitido pelo Azure Active Directory.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b9b9f75e55c027ecee0189b4ace2fd52e3d10e78
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158076"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="e43df-103">Tipo de recurso tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e43df-103">tokenLifetimePolicy resource type</span></span>

<span data-ttu-id="e43df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e43df-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="e43df-105">Representa uma política que pode controlar o tempo de vida de um token de acesso JWT, um token de ID ou um token SAML 1.1/2.0 emitido pelo Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="e43df-105">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="e43df-106">É possível definir tempos de vida do token para todos os aplicativos em sua organização, para um aplicativo multilocatário (organização múltipla) ou para uma entidade de serviço específica em sua organização.</span><span class="sxs-lookup"><span data-stu-id="e43df-106">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span>  <span data-ttu-id="e43df-107">Para obter mais detalhes do cenário, [consulte Tempo de vida de token configurável no Azure Active Directory.](/azure/active-directory/develop/active-directory-configurable-token-lifetimes)</span><span class="sxs-lookup"><span data-stu-id="e43df-107">For more scenario details see [Configurable token lifetimes in Azure Active Directory](/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

><span data-ttu-id="e43df-108">**Observação:** A configuração dessa política para Tokens de Atualização e Tokens de Sessão não é suportada.</span><span class="sxs-lookup"><span data-stu-id="e43df-108">**Note:** Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="e43df-109">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e43df-109">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e43df-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="e43df-110">Methods</span></span>

| <span data-ttu-id="e43df-111">Método</span><span class="sxs-lookup"><span data-stu-id="e43df-111">Method</span></span>       | <span data-ttu-id="e43df-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e43df-112">Return Type</span></span> | <span data-ttu-id="e43df-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="e43df-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e43df-114">Listar tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="e43df-114">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="e43df-115">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e43df-115">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="e43df-116">Leia as propriedades e os relacionamentos dos objetos tokenLifetimePolicies.</span><span class="sxs-lookup"><span data-stu-id="e43df-116">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="e43df-117">Criar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e43df-117">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="e43df-118">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e43df-118">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="e43df-119">Crie um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="e43df-119">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="e43df-120">Obter tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e43df-120">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="e43df-121">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e43df-121">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="e43df-122">Ler propriedades e relações de um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="e43df-122">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="e43df-123">Atualizar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e43df-123">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="e43df-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e43df-124">None</span></span> | <span data-ttu-id="e43df-125">Atualize um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="e43df-125">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="e43df-126">Excluir tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e43df-126">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="e43df-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e43df-127">None</span></span> | <span data-ttu-id="e43df-128">Exclua um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="e43df-128">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="e43df-129">Lista appliesTo</span><span class="sxs-lookup"><span data-stu-id="e43df-129">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="e43df-130">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="e43df-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="e43df-131">Obter a lista de directoryObjects aos qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="e43df-131">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="e43df-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e43df-132">Properties</span></span>

| <span data-ttu-id="e43df-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e43df-133">Property</span></span>     | <span data-ttu-id="e43df-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="e43df-134">Type</span></span>        | <span data-ttu-id="e43df-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="e43df-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e43df-136">id</span><span class="sxs-lookup"><span data-stu-id="e43df-136">id</span></span>|<span data-ttu-id="e43df-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e43df-137">String</span></span>| <span data-ttu-id="e43df-138">Identificador exclusivo desta política.</span><span class="sxs-lookup"><span data-stu-id="e43df-138">Unique identifier for this policy.</span></span> <span data-ttu-id="e43df-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e43df-139">Read-only.</span></span>|
|<span data-ttu-id="e43df-140">definição</span><span class="sxs-lookup"><span data-stu-id="e43df-140">definition</span></span>|<span data-ttu-id="e43df-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e43df-141">String collection</span></span>| <span data-ttu-id="e43df-142">Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política.</span><span class="sxs-lookup"><span data-stu-id="e43df-142">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="e43df-143">Veja abaixo para obter mais detalhes sobre o esquema JSON para essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="e43df-143">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="e43df-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e43df-144">Required.</span></span>|
|<span data-ttu-id="e43df-145">description</span><span class="sxs-lookup"><span data-stu-id="e43df-145">description</span></span>|<span data-ttu-id="e43df-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e43df-146">String</span></span>| <span data-ttu-id="e43df-147">Descrição desta política.</span><span class="sxs-lookup"><span data-stu-id="e43df-147">Description for this policy.</span></span>|
|<span data-ttu-id="e43df-148">displayName</span><span class="sxs-lookup"><span data-stu-id="e43df-148">displayName</span></span>|<span data-ttu-id="e43df-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e43df-149">String</span></span>| <span data-ttu-id="e43df-150">Nome para exibição desta política.</span><span class="sxs-lookup"><span data-stu-id="e43df-150">Display name for this policy.</span></span> <span data-ttu-id="e43df-151">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e43df-151">Required.</span></span>|
|<span data-ttu-id="e43df-152">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="e43df-152">isOrganizationDefault</span></span>|<span data-ttu-id="e43df-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="e43df-153">Boolean</span></span>|<span data-ttu-id="e43df-154">Se definido como true, ativa essa política.</span><span class="sxs-lookup"><span data-stu-id="e43df-154">If set to true, activates this policy.</span></span> <span data-ttu-id="e43df-155">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="e43df-155">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="e43df-156">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="e43df-156">Optional, default value is false.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="e43df-157">Propriedades de uma definição de política de tempo de vida do token</span><span class="sxs-lookup"><span data-stu-id="e43df-157">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="e43df-158">As propriedades abaixo formam o objeto JSON que representa uma política de tempo de vida do token.</span><span class="sxs-lookup"><span data-stu-id="e43df-158">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="e43df-159">Esse objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas que** não devem ser inseridas na propriedade de **definição.**</span><span class="sxs-lookup"><span data-stu-id="e43df-159">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="e43df-160">Um exemplo é mostrado abaixo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="e43df-160">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="e43df-161">**Observação:** Todas as durações de tempo nessas propriedades são especificadas no formato "dd.hh:mm:ss".</span><span class="sxs-lookup"><span data-stu-id="e43df-161">**Note:** All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="e43df-162">**Observação:** Os valores máximos para propriedades anotadas em "dias" são 1 segundo a menos do número de dias anotado.</span><span class="sxs-lookup"><span data-stu-id="e43df-162">**Note:** Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="e43df-163">Por exemplo, o valor máximo de 1 dia é especificado como "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="e43df-163">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="e43df-164">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e43df-164">Property</span></span>     | <span data-ttu-id="e43df-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="e43df-165">Type</span></span>   |<span data-ttu-id="e43df-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="e43df-166">Description</span></span>| <span data-ttu-id="e43df-167">Valor Mínimo</span><span class="sxs-lookup"><span data-stu-id="e43df-167">Min Value</span></span> | <span data-ttu-id="e43df-168">Valor Máximo</span><span class="sxs-lookup"><span data-stu-id="e43df-168">Max Value</span></span> | <span data-ttu-id="e43df-169">Valor padrão</span><span class="sxs-lookup"><span data-stu-id="e43df-169">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="e43df-170">AccessTokenLifetime</span><span class="sxs-lookup"><span data-stu-id="e43df-170">AccessTokenLifetime</span></span>|<span data-ttu-id="e43df-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e43df-171">String</span></span>|<span data-ttu-id="e43df-172">Controla por quanto tempo os tokens de acesso e de ID são considerados válidos.</span><span class="sxs-lookup"><span data-stu-id="e43df-172">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="e43df-173">10 minutos</span><span class="sxs-lookup"><span data-stu-id="e43df-173">10 minutes</span></span>|<span data-ttu-id="e43df-174">1 dia</span><span class="sxs-lookup"><span data-stu-id="e43df-174">1 day</span></span>|<span data-ttu-id="e43df-175">1 hora</span><span class="sxs-lookup"><span data-stu-id="e43df-175">1 hour</span></span>|
|<span data-ttu-id="e43df-176">Versão</span><span class="sxs-lookup"><span data-stu-id="e43df-176">Version</span></span>|<span data-ttu-id="e43df-177">Inteiro</span><span class="sxs-lookup"><span data-stu-id="e43df-177">Integer</span></span>|<span data-ttu-id="e43df-178">Valor definido de 1.</span><span class="sxs-lookup"><span data-stu-id="e43df-178">Set value of 1.</span></span> <span data-ttu-id="e43df-179">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e43df-179">Required.</span></span>|<span data-ttu-id="e43df-180">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e43df-180">None</span></span>|<span data-ttu-id="e43df-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e43df-181">None</span></span>|<span data-ttu-id="e43df-182">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e43df-182">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="e43df-183">Relações</span><span class="sxs-lookup"><span data-stu-id="e43df-183">Relationships</span></span>

| <span data-ttu-id="e43df-184">Relação</span><span class="sxs-lookup"><span data-stu-id="e43df-184">Relationship</span></span> | <span data-ttu-id="e43df-185">Tipo</span><span class="sxs-lookup"><span data-stu-id="e43df-185">Type</span></span>        | <span data-ttu-id="e43df-186">Descrição</span><span class="sxs-lookup"><span data-stu-id="e43df-186">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e43df-187">appliesTo</span><span class="sxs-lookup"><span data-stu-id="e43df-187">appliesTo</span></span>|<span data-ttu-id="e43df-188">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="e43df-188">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="e43df-189">A [coleção directoryObject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="e43df-189">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="e43df-190">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e43df-190">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e43df-191">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e43df-191">JSON representation</span></span>

<span data-ttu-id="e43df-192">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e43df-192">The following is a JSON representation of the resource.</span></span>

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