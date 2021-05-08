---
title: Tipo de recurso tokenLifetimePolicy
description: Representa uma política que pode controlar o tempo de vida de um token de acesso emitido por Azure Active Directory.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d143faa87af81fbaae73973510bafe3fd3ee4fcb
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241041"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="71237-103">Tipo de recurso tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="71237-103">tokenLifetimePolicy resource type</span></span>

<span data-ttu-id="71237-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71237-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="71237-105">Representa uma política que pode controlar o tempo de vida de um token de acesso JWT, um token de ID ou um token SAML 1.1/2.0 emitido pelo Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="71237-105">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="71237-106">É possível definir tempos de vida do token para todos os aplicativos em sua organização, para um aplicativo multilocatário (organização múltipla) ou para uma entidade de serviço específica em sua organização.</span><span class="sxs-lookup"><span data-stu-id="71237-106">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> 

><span data-ttu-id="71237-107">**Observação:** Não há suporte para configurar essa política para Tokens de Atualização e Tokens de Sessão.</span><span class="sxs-lookup"><span data-stu-id="71237-107">**Note:** Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="71237-108">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="71237-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="71237-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="71237-109">Methods</span></span>

| <span data-ttu-id="71237-110">Método</span><span class="sxs-lookup"><span data-stu-id="71237-110">Method</span></span>       | <span data-ttu-id="71237-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="71237-111">Return Type</span></span> | <span data-ttu-id="71237-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="71237-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="71237-113">Listar tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="71237-113">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="71237-114">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="71237-114">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="71237-115">Leia propriedades e relações de objetos tokenLifetimePolicies.</span><span class="sxs-lookup"><span data-stu-id="71237-115">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="71237-116">Criar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="71237-116">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="71237-117">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="71237-117">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="71237-118">Crie um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="71237-118">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="71237-119">Obter tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="71237-119">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="71237-120">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="71237-120">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="71237-121">Ler propriedades e relações de um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="71237-121">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="71237-122">Atualizar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="71237-122">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="71237-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71237-123">None</span></span> | <span data-ttu-id="71237-124">Atualize um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="71237-124">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="71237-125">Excluir tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="71237-125">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="71237-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71237-126">None</span></span> | <span data-ttu-id="71237-127">Exclua um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="71237-127">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="71237-128">Lista appliesTo</span><span class="sxs-lookup"><span data-stu-id="71237-128">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="71237-129">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="71237-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="71237-130">Obter a lista de directoryObjects aos qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="71237-130">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="71237-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71237-131">Properties</span></span>

| <span data-ttu-id="71237-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71237-132">Property</span></span>     | <span data-ttu-id="71237-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="71237-133">Type</span></span>        | <span data-ttu-id="71237-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="71237-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="71237-135">id</span><span class="sxs-lookup"><span data-stu-id="71237-135">id</span></span>|<span data-ttu-id="71237-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71237-136">String</span></span>| <span data-ttu-id="71237-137">Identificador exclusivo dessa política.</span><span class="sxs-lookup"><span data-stu-id="71237-137">Unique identifier for this policy.</span></span> <span data-ttu-id="71237-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71237-138">Read-only.</span></span>|
|<span data-ttu-id="71237-139">definition</span><span class="sxs-lookup"><span data-stu-id="71237-139">definition</span></span>|<span data-ttu-id="71237-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="71237-140">String collection</span></span>| <span data-ttu-id="71237-141">Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política.</span><span class="sxs-lookup"><span data-stu-id="71237-141">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="71237-142">Consulte abaixo para obter mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="71237-142">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="71237-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71237-143">Required.</span></span>|
|<span data-ttu-id="71237-144">description</span><span class="sxs-lookup"><span data-stu-id="71237-144">description</span></span>|<span data-ttu-id="71237-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71237-145">String</span></span>| <span data-ttu-id="71237-146">Descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="71237-146">Description for this policy.</span></span>|
|<span data-ttu-id="71237-147">displayName</span><span class="sxs-lookup"><span data-stu-id="71237-147">displayName</span></span>|<span data-ttu-id="71237-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71237-148">String</span></span>| <span data-ttu-id="71237-149">Nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="71237-149">Display name for this policy.</span></span> <span data-ttu-id="71237-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71237-150">Required.</span></span>|
|<span data-ttu-id="71237-151">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="71237-151">isOrganizationDefault</span></span>|<span data-ttu-id="71237-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="71237-152">Boolean</span></span>|<span data-ttu-id="71237-153">Se definido como `true` , ativa essa política.</span><span class="sxs-lookup"><span data-stu-id="71237-153">If set to `true`, activates this policy.</span></span> <span data-ttu-id="71237-154">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como o padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="71237-154">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="71237-155">Opcional, o valor padrão é `false` .</span><span class="sxs-lookup"><span data-stu-id="71237-155">Optional, default value is `false`.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="71237-156">Propriedades de uma definição de política de vida útil do token</span><span class="sxs-lookup"><span data-stu-id="71237-156">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="71237-157">As propriedades abaixo formam o objeto JSON que representa uma política de vida útil do token.</span><span class="sxs-lookup"><span data-stu-id="71237-157">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="71237-158">Esse objeto JSON deve ser **convertido em uma cadeia de caracteres com** aspas que escapam para serem inseridas na propriedade **definition.**</span><span class="sxs-lookup"><span data-stu-id="71237-158">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="71237-159">Um exemplo é mostrado abaixo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="71237-159">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="71237-160">**Observação:** Todas as durações de tempo nessas propriedades são especificadas no formato "dd.hh:mm:ss".</span><span class="sxs-lookup"><span data-stu-id="71237-160">**Note:** All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="71237-161">**Observação:** Os valores máximos para propriedades anotadas em "dias" são 1 segundo a menos do número de dias anotado.</span><span class="sxs-lookup"><span data-stu-id="71237-161">**Note:** Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="71237-162">Por exemplo, o valor máximo de 1 dia é especificado como "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="71237-162">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="71237-163">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71237-163">Property</span></span>     | <span data-ttu-id="71237-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="71237-164">Type</span></span>   |<span data-ttu-id="71237-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="71237-165">Description</span></span>| <span data-ttu-id="71237-166">Valor Mínimo</span><span class="sxs-lookup"><span data-stu-id="71237-166">Min Value</span></span> | <span data-ttu-id="71237-167">Valor Máximo</span><span class="sxs-lookup"><span data-stu-id="71237-167">Max Value</span></span> | <span data-ttu-id="71237-168">Valor padrão</span><span class="sxs-lookup"><span data-stu-id="71237-168">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="71237-169">AccessTokenLifetime</span><span class="sxs-lookup"><span data-stu-id="71237-169">AccessTokenLifetime</span></span>|<span data-ttu-id="71237-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71237-170">String</span></span>|<span data-ttu-id="71237-171">Controla por quanto tempo os tokens de acesso e ID são considerados válidos.</span><span class="sxs-lookup"><span data-stu-id="71237-171">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="71237-172">10 minutos</span><span class="sxs-lookup"><span data-stu-id="71237-172">10 minutes</span></span>|<span data-ttu-id="71237-173">1 dia</span><span class="sxs-lookup"><span data-stu-id="71237-173">1 day</span></span>|<span data-ttu-id="71237-174">1 hora</span><span class="sxs-lookup"><span data-stu-id="71237-174">1 hour</span></span>|
|<span data-ttu-id="71237-175">Versão</span><span class="sxs-lookup"><span data-stu-id="71237-175">Version</span></span>|<span data-ttu-id="71237-176">Inteiro</span><span class="sxs-lookup"><span data-stu-id="71237-176">Integer</span></span>|<span data-ttu-id="71237-177">Definir o valor de 1.</span><span class="sxs-lookup"><span data-stu-id="71237-177">Set value of 1.</span></span> <span data-ttu-id="71237-178">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71237-178">Required.</span></span>|<span data-ttu-id="71237-179">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71237-179">None</span></span>|<span data-ttu-id="71237-180">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71237-180">None</span></span>|<span data-ttu-id="71237-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71237-181">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="71237-182">Relações</span><span class="sxs-lookup"><span data-stu-id="71237-182">Relationships</span></span>

| <span data-ttu-id="71237-183">Relação</span><span class="sxs-lookup"><span data-stu-id="71237-183">Relationship</span></span> | <span data-ttu-id="71237-184">Tipo</span><span class="sxs-lookup"><span data-stu-id="71237-184">Type</span></span>        | <span data-ttu-id="71237-185">Descrição</span><span class="sxs-lookup"><span data-stu-id="71237-185">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="71237-186">appliesTo</span><span class="sxs-lookup"><span data-stu-id="71237-186">appliesTo</span></span>|<span data-ttu-id="71237-187">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="71237-187">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="71237-188">A [coleção directoryObject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="71237-188">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="71237-189">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71237-189">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71237-190">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71237-190">JSON representation</span></span>

<span data-ttu-id="71237-191">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71237-191">The following is a JSON representation of the resource.</span></span>

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
