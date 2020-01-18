---
title: tipo de recurso tokenLifetimePolicy
description: Representa uma política que pode controlar o tempo de vida de um token de acesso emitido pelo Azure Active Directory.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6a19ec9e2b8747737895bed89b1a92ec4c5d134a
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234116"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="e3d9f-103">tipo de recurso tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e3d9f-103">tokenLifetimePolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3d9f-104">Representa uma política que pode controlar o tempo de vida de um token de acesso JWT, um token de ID ou um token SAML 1.1/2.0 emitido pelo Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="e3d9f-104">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="e3d9f-105">Você pode definir vidas úteis de token para todos os aplicativos em sua organização, para um aplicativo multilocatário (várias organizações) ou para uma entidade de serviço específica em sua organização.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-105">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span>  <span data-ttu-id="e3d9f-106">Para obter mais detalhes do cenário, consulte [tempos de vida de token configuráveis no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="e3d9f-106">For more scenario details see [Configurable token lifetimes in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

><span data-ttu-id="e3d9f-107">Observação: não há suporte para a configuração dessa política para tokens de atualização e de sessão.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-107">Note: Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="e3d9f-108">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e3d9f-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e3d9f-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="e3d9f-109">Methods</span></span>

| <span data-ttu-id="e3d9f-110">Método</span><span class="sxs-lookup"><span data-stu-id="e3d9f-110">Method</span></span>       | <span data-ttu-id="e3d9f-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e3d9f-111">Return Type</span></span> | <span data-ttu-id="e3d9f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3d9f-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e3d9f-113">Criar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e3d9f-113">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="e3d9f-114">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e3d9f-114">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="e3d9f-115">Criar um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-115">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="e3d9f-116">Obter tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e3d9f-116">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="e3d9f-117">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e3d9f-117">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="e3d9f-118">Ler propriedades e relações de um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-118">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="e3d9f-119">Listar tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="e3d9f-119">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="e3d9f-120">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e3d9f-120">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="e3d9f-121">Ler propriedades e relações de objetos tokenLifetimePolicies.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-121">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="e3d9f-122">Atualizar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e3d9f-122">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="e3d9f-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e3d9f-123">None</span></span> | <span data-ttu-id="e3d9f-124">Atualizar um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-124">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="e3d9f-125">Excluir tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="e3d9f-125">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="e3d9f-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e3d9f-126">None</span></span> | <span data-ttu-id="e3d9f-127">Excluir um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-127">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="e3d9f-128">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="e3d9f-128">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="e3d9f-129">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="e3d9f-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="e3d9f-130">Obtenha a lista de directoryObjects à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-130">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="e3d9f-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3d9f-131">Properties</span></span>

| <span data-ttu-id="e3d9f-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3d9f-132">Property</span></span>     | <span data-ttu-id="e3d9f-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3d9f-133">Type</span></span>        | <span data-ttu-id="e3d9f-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3d9f-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e3d9f-135">id</span><span class="sxs-lookup"><span data-stu-id="e3d9f-135">id</span></span>|<span data-ttu-id="e3d9f-136">String</span><span class="sxs-lookup"><span data-stu-id="e3d9f-136">String</span></span>| <span data-ttu-id="e3d9f-137">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-137">Unique identifier for this policy.</span></span> <span data-ttu-id="e3d9f-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-138">Read-only.</span></span>|
|<span data-ttu-id="e3d9f-139">definir</span><span class="sxs-lookup"><span data-stu-id="e3d9f-139">definition</span></span>|<span data-ttu-id="e3d9f-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3d9f-140">String collection</span></span>| <span data-ttu-id="e3d9f-141">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-141">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="e3d9f-142">Veja mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-142">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="e3d9f-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-143">Required.</span></span>|
|<span data-ttu-id="e3d9f-144">description</span><span class="sxs-lookup"><span data-stu-id="e3d9f-144">description</span></span>|<span data-ttu-id="e3d9f-145">String</span><span class="sxs-lookup"><span data-stu-id="e3d9f-145">String</span></span>| <span data-ttu-id="e3d9f-146">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-146">Description for this policy.</span></span>|
|<span data-ttu-id="e3d9f-147">displayName</span><span class="sxs-lookup"><span data-stu-id="e3d9f-147">displayName</span></span>|<span data-ttu-id="e3d9f-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3d9f-148">String</span></span>| <span data-ttu-id="e3d9f-149">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-149">Display name for this policy.</span></span> <span data-ttu-id="e3d9f-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-150">Required.</span></span>|
|<span data-ttu-id="e3d9f-151">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="e3d9f-151">isOrganizationDefault</span></span>|<span data-ttu-id="e3d9f-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="e3d9f-152">Boolean</span></span>|<span data-ttu-id="e3d9f-153">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-153">If set to true, activates this policy.</span></span> <span data-ttu-id="e3d9f-154">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-154">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="e3d9f-155">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-155">Optional, default value is false.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="e3d9f-156">Propriedades de uma definição de política de tempo de vida do token</span><span class="sxs-lookup"><span data-stu-id="e3d9f-156">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="e3d9f-157">As propriedades abaixo formam o objeto JSON que representa uma política de tempo de vida do token.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-157">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="e3d9f-158">Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** .</span><span class="sxs-lookup"><span data-stu-id="e3d9f-158">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="e3d9f-159">Um exemplo é mostrado abaixo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="e3d9f-159">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="e3d9f-160">Observação: todas as durações de tempo nessas propriedades são especificadas no formato "dd. hh: mm: SS".</span><span class="sxs-lookup"><span data-stu-id="e3d9f-160">Note: All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="e3d9f-161">Observação: os valores máximos para propriedades denotadas em "dias" são 1 segundo curto do número de dias indicado.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-161">Note: Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="e3d9f-162">Por exemplo, o valor máximo de 1 dia é especificado como "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="e3d9f-162">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="e3d9f-163">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3d9f-163">Property</span></span>     | <span data-ttu-id="e3d9f-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3d9f-164">Type</span></span>   |<span data-ttu-id="e3d9f-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3d9f-165">Description</span></span>| <span data-ttu-id="e3d9f-166">Valor mínimo</span><span class="sxs-lookup"><span data-stu-id="e3d9f-166">Min Value</span></span> | <span data-ttu-id="e3d9f-167">Valor máximo</span><span class="sxs-lookup"><span data-stu-id="e3d9f-167">Max Value</span></span> | <span data-ttu-id="e3d9f-168">Valor padrão</span><span class="sxs-lookup"><span data-stu-id="e3d9f-168">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="e3d9f-169">AccessTokenLifetime</span><span class="sxs-lookup"><span data-stu-id="e3d9f-169">AccessTokenLifetime</span></span>|<span data-ttu-id="e3d9f-170">String</span><span class="sxs-lookup"><span data-stu-id="e3d9f-170">String</span></span>|<span data-ttu-id="e3d9f-171">Controla por quanto tempo os tokens de acesso e de ID são considerados válidos.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-171">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="e3d9f-172">10 minutos</span><span class="sxs-lookup"><span data-stu-id="e3d9f-172">10 minutes</span></span>|<span data-ttu-id="e3d9f-173">1 dia</span><span class="sxs-lookup"><span data-stu-id="e3d9f-173">1 day</span></span>|<span data-ttu-id="e3d9f-174">1 hour</span><span class="sxs-lookup"><span data-stu-id="e3d9f-174">1 hour</span></span>|
|<span data-ttu-id="e3d9f-175">Versão</span><span class="sxs-lookup"><span data-stu-id="e3d9f-175">Version</span></span>|<span data-ttu-id="e3d9f-176">Inteiro</span><span class="sxs-lookup"><span data-stu-id="e3d9f-176">Integer</span></span>|<span data-ttu-id="e3d9f-177">Defina o valor 1.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-177">Set value of 1.</span></span> <span data-ttu-id="e3d9f-178">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-178">Required.</span></span>|<span data-ttu-id="e3d9f-179">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e3d9f-179">None</span></span>|<span data-ttu-id="e3d9f-180">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e3d9f-180">None</span></span>|<span data-ttu-id="e3d9f-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e3d9f-181">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3d9f-182">Relações</span><span class="sxs-lookup"><span data-stu-id="e3d9f-182">Relationships</span></span>

| <span data-ttu-id="e3d9f-183">Relação</span><span class="sxs-lookup"><span data-stu-id="e3d9f-183">Relationship</span></span> | <span data-ttu-id="e3d9f-184">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3d9f-184">Type</span></span>        | <span data-ttu-id="e3d9f-185">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3d9f-185">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e3d9f-186">appliesTo</span><span class="sxs-lookup"><span data-stu-id="e3d9f-186">appliesTo</span></span>|<span data-ttu-id="e3d9f-187">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="e3d9f-187">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="e3d9f-188">A coleção [directoryobject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-188">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="e3d9f-189">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-189">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3d9f-190">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3d9f-190">JSON representation</span></span>

<span data-ttu-id="e3d9f-191">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3d9f-191">The following is a JSON representation of the resource.</span></span>

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