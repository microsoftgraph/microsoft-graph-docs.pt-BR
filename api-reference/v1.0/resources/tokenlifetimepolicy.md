---
title: tipo de recurso tokenLifetimePolicy
description: Representa uma política que pode controlar o tempo de vida de um token de acesso emitido pelo Azure Active Directory.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 568d8244170ade5c2e6a9faebcd910d0470635ef
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229637"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="08729-103">tipo de recurso tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="08729-103">tokenLifetimePolicy resource type</span></span>

<span data-ttu-id="08729-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08729-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="08729-105">Representa uma política que pode controlar o tempo de vida de um token de acesso JWT, um token de ID ou um token SAML 1.1/2.0 emitido pelo Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="08729-105">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="08729-106">Você pode definir vidas úteis de token para todos os aplicativos em sua organização, para um aplicativo multilocatário (várias organizações) ou para uma entidade de serviço específica em sua organização.</span><span class="sxs-lookup"><span data-stu-id="08729-106">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span>  <span data-ttu-id="08729-107">Para obter mais detalhes do cenário, consulte [tempos de vida de token configuráveis no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="08729-107">For more scenario details see [Configurable token lifetimes in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

><span data-ttu-id="08729-108">**Observação:** Não há suporte para a configuração dessa política para tokens de atualização e de sessão.</span><span class="sxs-lookup"><span data-stu-id="08729-108">**Note:** Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="08729-109">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="08729-109">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="08729-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="08729-110">Methods</span></span>

| <span data-ttu-id="08729-111">Método</span><span class="sxs-lookup"><span data-stu-id="08729-111">Method</span></span>       | <span data-ttu-id="08729-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="08729-112">Return Type</span></span> | <span data-ttu-id="08729-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="08729-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="08729-114">Listar tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="08729-114">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="08729-115">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="08729-115">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="08729-116">Ler propriedades e relações de objetos tokenLifetimePolicies.</span><span class="sxs-lookup"><span data-stu-id="08729-116">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="08729-117">Criar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="08729-117">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="08729-118">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="08729-118">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="08729-119">Criar um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="08729-119">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="08729-120">Obter tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="08729-120">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="08729-121">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="08729-121">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="08729-122">Ler propriedades e relações de um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="08729-122">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="08729-123">Atualizar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="08729-123">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="08729-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08729-124">None</span></span> | <span data-ttu-id="08729-125">Atualizar um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="08729-125">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="08729-126">Excluir tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="08729-126">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="08729-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08729-127">None</span></span> | <span data-ttu-id="08729-128">Excluir um objeto tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="08729-128">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="08729-129">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="08729-129">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="08729-130">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="08729-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="08729-131">Obtenha a lista de directoryObjects à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="08729-131">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="08729-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08729-132">Properties</span></span>

| <span data-ttu-id="08729-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08729-133">Property</span></span>     | <span data-ttu-id="08729-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="08729-134">Type</span></span>        | <span data-ttu-id="08729-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="08729-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="08729-136">id</span><span class="sxs-lookup"><span data-stu-id="08729-136">id</span></span>|<span data-ttu-id="08729-137">String</span><span class="sxs-lookup"><span data-stu-id="08729-137">String</span></span>| <span data-ttu-id="08729-138">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="08729-138">Unique identifier for this policy.</span></span> <span data-ttu-id="08729-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="08729-139">Read-only.</span></span>|
|<span data-ttu-id="08729-140">definir</span><span class="sxs-lookup"><span data-stu-id="08729-140">definition</span></span>|<span data-ttu-id="08729-141">String collection</span><span class="sxs-lookup"><span data-stu-id="08729-141">String collection</span></span>| <span data-ttu-id="08729-142">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="08729-142">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="08729-143">Veja mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="08729-143">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="08729-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08729-144">Required.</span></span>|
|<span data-ttu-id="08729-145">description</span><span class="sxs-lookup"><span data-stu-id="08729-145">description</span></span>|<span data-ttu-id="08729-146">String</span><span class="sxs-lookup"><span data-stu-id="08729-146">String</span></span>| <span data-ttu-id="08729-147">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="08729-147">Description for this policy.</span></span>|
|<span data-ttu-id="08729-148">displayName</span><span class="sxs-lookup"><span data-stu-id="08729-148">displayName</span></span>|<span data-ttu-id="08729-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08729-149">String</span></span>| <span data-ttu-id="08729-150">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="08729-150">Display name for this policy.</span></span> <span data-ttu-id="08729-151">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08729-151">Required.</span></span>|
|<span data-ttu-id="08729-152">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="08729-152">isOrganizationDefault</span></span>|<span data-ttu-id="08729-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="08729-153">Boolean</span></span>|<span data-ttu-id="08729-154">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="08729-154">If set to true, activates this policy.</span></span> <span data-ttu-id="08729-155">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="08729-155">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="08729-156">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="08729-156">Optional, default value is false.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="08729-157">Propriedades de uma definição de política de tempo de vida do token</span><span class="sxs-lookup"><span data-stu-id="08729-157">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="08729-158">As propriedades abaixo formam o objeto JSON que representa uma política de tempo de vida do token.</span><span class="sxs-lookup"><span data-stu-id="08729-158">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="08729-159">Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** .</span><span class="sxs-lookup"><span data-stu-id="08729-159">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="08729-160">Um exemplo é mostrado abaixo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="08729-160">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="08729-161">**Observação:** Todas as durações de tempo nessas propriedades são especificadas no formato "dd. hh: mm: SS".</span><span class="sxs-lookup"><span data-stu-id="08729-161">**Note:** All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="08729-162">**Observação:** Os valores máximos para propriedades indicados em "dias" são 1 segundo curto do número de dias indicado.</span><span class="sxs-lookup"><span data-stu-id="08729-162">**Note:** Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="08729-163">Por exemplo, o valor máximo de 1 dia é especificado como "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="08729-163">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="08729-164">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08729-164">Property</span></span>     | <span data-ttu-id="08729-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="08729-165">Type</span></span>   |<span data-ttu-id="08729-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="08729-166">Description</span></span>| <span data-ttu-id="08729-167">Valor mínimo</span><span class="sxs-lookup"><span data-stu-id="08729-167">Min Value</span></span> | <span data-ttu-id="08729-168">Valor máximo</span><span class="sxs-lookup"><span data-stu-id="08729-168">Max Value</span></span> | <span data-ttu-id="08729-169">Valor padrão</span><span class="sxs-lookup"><span data-stu-id="08729-169">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="08729-170">AccessTokenLifetime</span><span class="sxs-lookup"><span data-stu-id="08729-170">AccessTokenLifetime</span></span>|<span data-ttu-id="08729-171">String</span><span class="sxs-lookup"><span data-stu-id="08729-171">String</span></span>|<span data-ttu-id="08729-172">Controla por quanto tempo os tokens de acesso e de ID são considerados válidos.</span><span class="sxs-lookup"><span data-stu-id="08729-172">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="08729-173">10 minutos</span><span class="sxs-lookup"><span data-stu-id="08729-173">10 minutes</span></span>|<span data-ttu-id="08729-174">1 dia</span><span class="sxs-lookup"><span data-stu-id="08729-174">1 day</span></span>|<span data-ttu-id="08729-175">1 hora</span><span class="sxs-lookup"><span data-stu-id="08729-175">1 hour</span></span>|
|<span data-ttu-id="08729-176">Versão</span><span class="sxs-lookup"><span data-stu-id="08729-176">Version</span></span>|<span data-ttu-id="08729-177">Inteiro</span><span class="sxs-lookup"><span data-stu-id="08729-177">Integer</span></span>|<span data-ttu-id="08729-178">Defina o valor 1.</span><span class="sxs-lookup"><span data-stu-id="08729-178">Set value of 1.</span></span> <span data-ttu-id="08729-179">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08729-179">Required.</span></span>|<span data-ttu-id="08729-180">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08729-180">None</span></span>|<span data-ttu-id="08729-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08729-181">None</span></span>|<span data-ttu-id="08729-182">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08729-182">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="08729-183">Relações</span><span class="sxs-lookup"><span data-stu-id="08729-183">Relationships</span></span>

| <span data-ttu-id="08729-184">Relação</span><span class="sxs-lookup"><span data-stu-id="08729-184">Relationship</span></span> | <span data-ttu-id="08729-185">Tipo</span><span class="sxs-lookup"><span data-stu-id="08729-185">Type</span></span>        | <span data-ttu-id="08729-186">Descrição</span><span class="sxs-lookup"><span data-stu-id="08729-186">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="08729-187">appliesTo</span><span class="sxs-lookup"><span data-stu-id="08729-187">appliesTo</span></span>|<span data-ttu-id="08729-188">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="08729-188">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="08729-189">A coleção [directoryobject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="08729-189">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="08729-190">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="08729-190">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08729-191">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08729-191">JSON representation</span></span>

<span data-ttu-id="08729-192">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08729-192">The following is a JSON representation of the resource.</span></span>

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
