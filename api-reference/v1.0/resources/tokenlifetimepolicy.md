---
title: Tipo de recurso tokenLifetimePolicy
description: Representa uma política que pode controlar o tempo de vida de um token de acesso emitido pelo Azure Active Directory.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b4d8d814278855e164fa00643b8f56ebc544a789
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963355"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="72684-103">Tipo de recurso tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="72684-103">tokenLifetimePolicy resource type</span></span>

<span data-ttu-id="72684-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72684-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="72684-105">Representa uma política que pode controlar o tempo de vida de um token de acesso JWT, um token de ID ou um token SAML 1.1/2.0 emitido pelo Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="72684-105">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="72684-106">É possível definir tempos de vida do token para todos os aplicativos em sua organização, para um aplicativo multilocatário (organização múltipla) ou para uma entidade de serviço específica em sua organização.</span><span class="sxs-lookup"><span data-stu-id="72684-106">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span>  <span data-ttu-id="72684-107">Para obter mais detalhes do cenário, [consulte Tempo de vida útil do token configurável no Azure Active Directory](/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="72684-107">For more scenario details see [Configurable token lifetimes in Azure Active Directory](/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

><span data-ttu-id="72684-108">**Observação:** Não há suporte para configurar essa política para Tokens de Atualização e Tokens de Sessão.</span><span class="sxs-lookup"><span data-stu-id="72684-108">**Note:** Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="72684-109">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="72684-109">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="72684-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="72684-110">Methods</span></span>

| <span data-ttu-id="72684-111">Método</span><span class="sxs-lookup"><span data-stu-id="72684-111">Method</span></span>       | <span data-ttu-id="72684-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="72684-112">Return Type</span></span> | <span data-ttu-id="72684-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="72684-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="72684-114">Listar tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="72684-114">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="72684-115">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="72684-115">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="72684-116">Leia propriedades e relações de objetos tokenLifetimePolicies.</span><span class="sxs-lookup"><span data-stu-id="72684-116">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="72684-117">Criar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="72684-117">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="72684-118">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="72684-118">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="72684-119">Crie um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="72684-119">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="72684-120">Obter tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="72684-120">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="72684-121">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="72684-121">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="72684-122">Ler propriedades e relações de um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="72684-122">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="72684-123">Atualizar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="72684-123">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="72684-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="72684-124">None</span></span> | <span data-ttu-id="72684-125">Atualize um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="72684-125">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="72684-126">Excluir tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="72684-126">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="72684-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="72684-127">None</span></span> | <span data-ttu-id="72684-128">Exclua um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="72684-128">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="72684-129">Lista appliesTo</span><span class="sxs-lookup"><span data-stu-id="72684-129">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="72684-130">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="72684-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="72684-131">Obter a lista de directoryObjects aos qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="72684-131">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="72684-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="72684-132">Properties</span></span>

| <span data-ttu-id="72684-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72684-133">Property</span></span>     | <span data-ttu-id="72684-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="72684-134">Type</span></span>        | <span data-ttu-id="72684-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="72684-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="72684-136">id</span><span class="sxs-lookup"><span data-stu-id="72684-136">id</span></span>|<span data-ttu-id="72684-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72684-137">String</span></span>| <span data-ttu-id="72684-138">Identificador exclusivo dessa política.</span><span class="sxs-lookup"><span data-stu-id="72684-138">Unique identifier for this policy.</span></span> <span data-ttu-id="72684-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72684-139">Read-only.</span></span>|
|<span data-ttu-id="72684-140">definition</span><span class="sxs-lookup"><span data-stu-id="72684-140">definition</span></span>|<span data-ttu-id="72684-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="72684-141">String collection</span></span>| <span data-ttu-id="72684-142">Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política.</span><span class="sxs-lookup"><span data-stu-id="72684-142">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="72684-143">Consulte abaixo para obter mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="72684-143">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="72684-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72684-144">Required.</span></span>|
|<span data-ttu-id="72684-145">description</span><span class="sxs-lookup"><span data-stu-id="72684-145">description</span></span>|<span data-ttu-id="72684-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72684-146">String</span></span>| <span data-ttu-id="72684-147">Descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="72684-147">Description for this policy.</span></span>|
|<span data-ttu-id="72684-148">displayName</span><span class="sxs-lookup"><span data-stu-id="72684-148">displayName</span></span>|<span data-ttu-id="72684-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72684-149">String</span></span>| <span data-ttu-id="72684-150">Nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="72684-150">Display name for this policy.</span></span> <span data-ttu-id="72684-151">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72684-151">Required.</span></span>|
|<span data-ttu-id="72684-152">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="72684-152">isOrganizationDefault</span></span>|<span data-ttu-id="72684-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="72684-153">Boolean</span></span>|<span data-ttu-id="72684-154">Se definido como `true` , ativa essa política.</span><span class="sxs-lookup"><span data-stu-id="72684-154">If set to `true`, activates this policy.</span></span> <span data-ttu-id="72684-155">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como o padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="72684-155">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="72684-156">Opcional, o valor padrão é `false` .</span><span class="sxs-lookup"><span data-stu-id="72684-156">Optional, default value is `false`.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="72684-157">Propriedades de uma definição de política de vida útil do token</span><span class="sxs-lookup"><span data-stu-id="72684-157">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="72684-158">As propriedades abaixo formam o objeto JSON que representa uma política de vida útil do token.</span><span class="sxs-lookup"><span data-stu-id="72684-158">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="72684-159">Esse objeto JSON deve ser **convertido em uma cadeia de caracteres com** aspas que escapam para serem inseridas na propriedade **definition.**</span><span class="sxs-lookup"><span data-stu-id="72684-159">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="72684-160">Um exemplo é mostrado abaixo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="72684-160">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="72684-161">**Observação:** Todas as durações de tempo nessas propriedades são especificadas no formato "dd.hh:mm:ss".</span><span class="sxs-lookup"><span data-stu-id="72684-161">**Note:** All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="72684-162">**Observação:** Os valores máximos para propriedades anotadas em "dias" são 1 segundo a menos do número de dias anotado.</span><span class="sxs-lookup"><span data-stu-id="72684-162">**Note:** Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="72684-163">Por exemplo, o valor máximo de 1 dia é especificado como "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="72684-163">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="72684-164">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72684-164">Property</span></span>     | <span data-ttu-id="72684-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="72684-165">Type</span></span>   |<span data-ttu-id="72684-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="72684-166">Description</span></span>| <span data-ttu-id="72684-167">Valor Mínimo</span><span class="sxs-lookup"><span data-stu-id="72684-167">Min Value</span></span> | <span data-ttu-id="72684-168">Valor Máximo</span><span class="sxs-lookup"><span data-stu-id="72684-168">Max Value</span></span> | <span data-ttu-id="72684-169">Valor padrão</span><span class="sxs-lookup"><span data-stu-id="72684-169">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="72684-170">AccessTokenLifetime</span><span class="sxs-lookup"><span data-stu-id="72684-170">AccessTokenLifetime</span></span>|<span data-ttu-id="72684-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72684-171">String</span></span>|<span data-ttu-id="72684-172">Controla por quanto tempo os tokens de acesso e ID são considerados válidos.</span><span class="sxs-lookup"><span data-stu-id="72684-172">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="72684-173">10 minutos</span><span class="sxs-lookup"><span data-stu-id="72684-173">10 minutes</span></span>|<span data-ttu-id="72684-174">1 dia</span><span class="sxs-lookup"><span data-stu-id="72684-174">1 day</span></span>|<span data-ttu-id="72684-175">1 hora</span><span class="sxs-lookup"><span data-stu-id="72684-175">1 hour</span></span>|
|<span data-ttu-id="72684-176">Versão</span><span class="sxs-lookup"><span data-stu-id="72684-176">Version</span></span>|<span data-ttu-id="72684-177">Inteiro</span><span class="sxs-lookup"><span data-stu-id="72684-177">Integer</span></span>|<span data-ttu-id="72684-178">Definir o valor de 1.</span><span class="sxs-lookup"><span data-stu-id="72684-178">Set value of 1.</span></span> <span data-ttu-id="72684-179">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72684-179">Required.</span></span>|<span data-ttu-id="72684-180">Nenhum</span><span class="sxs-lookup"><span data-stu-id="72684-180">None</span></span>|<span data-ttu-id="72684-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="72684-181">None</span></span>|<span data-ttu-id="72684-182">Nenhum</span><span class="sxs-lookup"><span data-stu-id="72684-182">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="72684-183">Relações</span><span class="sxs-lookup"><span data-stu-id="72684-183">Relationships</span></span>

| <span data-ttu-id="72684-184">Relação</span><span class="sxs-lookup"><span data-stu-id="72684-184">Relationship</span></span> | <span data-ttu-id="72684-185">Tipo</span><span class="sxs-lookup"><span data-stu-id="72684-185">Type</span></span>        | <span data-ttu-id="72684-186">Descrição</span><span class="sxs-lookup"><span data-stu-id="72684-186">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="72684-187">appliesTo</span><span class="sxs-lookup"><span data-stu-id="72684-187">appliesTo</span></span>|<span data-ttu-id="72684-188">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="72684-188">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="72684-189">A [coleção directoryObject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="72684-189">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="72684-190">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72684-190">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="72684-191">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="72684-191">JSON representation</span></span>

<span data-ttu-id="72684-192">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="72684-192">The following is a JSON representation of the resource.</span></span>

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
