---
title: tipo de recurso tokenIssuancePolicy
description: Representa a política para especificar as características dos tokens SAML emitidos pelo Azure AD.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 030b05a7609b9588f0860471272c62007eaa1692
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229574"
---
# <a name="tokenissuancepolicy-resource-type"></a><span data-ttu-id="70509-103">tipo de recurso tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="70509-103">tokenIssuancePolicy resource type</span></span>

<span data-ttu-id="70509-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70509-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="70509-105">Representa a política para especificar as características dos tokens SAML emitidos pelo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="70509-105">Represents the policy to specify the characteristics of SAML tokens issued by Azure AD.</span></span> <span data-ttu-id="70509-106">Você pode usar as políticas de emissão de tokens para:</span><span class="sxs-lookup"><span data-stu-id="70509-106">You can use token-issuance policies to:</span></span>

- <span data-ttu-id="70509-107">Definir opções de assinatura</span><span class="sxs-lookup"><span data-stu-id="70509-107">Set signing options</span></span>
- <span data-ttu-id="70509-108">Definir algoritmo de assinatura</span><span class="sxs-lookup"><span data-stu-id="70509-108">Set signing algorithm</span></span>
- <span data-ttu-id="70509-109">Definir versão do token SAML</span><span class="sxs-lookup"><span data-stu-id="70509-109">Set SAML token version</span></span>

<span data-ttu-id="70509-110">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="70509-110">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="70509-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="70509-111">Methods</span></span>

| <span data-ttu-id="70509-112">Método</span><span class="sxs-lookup"><span data-stu-id="70509-112">Method</span></span>       | <span data-ttu-id="70509-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="70509-113">Return Type</span></span> | <span data-ttu-id="70509-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="70509-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="70509-115">Listar tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="70509-115">List tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-list.md) | [<span data-ttu-id="70509-116">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="70509-116">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="70509-117">Ler propriedades e relações de objetos tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="70509-117">Read properties and relationships of tokenIssuancePolicy objects.</span></span> |
| [<span data-ttu-id="70509-118">Criar tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="70509-118">Create tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-post-tokenissuancepolicy.md) | [<span data-ttu-id="70509-119">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="70509-119">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="70509-120">Criar um objeto tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="70509-120">Create a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="70509-121">Obter tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="70509-121">Get tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-get.md) | [<span data-ttu-id="70509-122">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="70509-122">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="70509-123">Ler propriedades e relações de um objeto tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="70509-123">Read properties and relationships of a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="70509-124">Atualizar tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="70509-124">Update tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-update.md) | <span data-ttu-id="70509-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70509-125">None</span></span> | <span data-ttu-id="70509-126">Atualizar um objeto tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="70509-126">Update a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="70509-127">Excluir tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="70509-127">Delete tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-delete.md) | <span data-ttu-id="70509-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70509-128">None</span></span> | <span data-ttu-id="70509-129">Excluir um objeto tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="70509-129">Delete a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="70509-130">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="70509-130">List appliesTo</span></span>](../api/tokenissuancepolicy-list-appliesto.md) | <span data-ttu-id="70509-131">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="70509-131">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="70509-132">Obtenha a lista de directoryObjects à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="70509-132">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="70509-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70509-133">Properties</span></span>

| <span data-ttu-id="70509-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70509-134">Property</span></span>     | <span data-ttu-id="70509-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="70509-135">Type</span></span>        | <span data-ttu-id="70509-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="70509-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="70509-137">id</span><span class="sxs-lookup"><span data-stu-id="70509-137">id</span></span>|<span data-ttu-id="70509-138">String</span><span class="sxs-lookup"><span data-stu-id="70509-138">String</span></span>| <span data-ttu-id="70509-139">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="70509-139">Unique identifier for this policy.</span></span> <span data-ttu-id="70509-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70509-140">Read-only.</span></span>|
|<span data-ttu-id="70509-141">definir</span><span class="sxs-lookup"><span data-stu-id="70509-141">definition</span></span>|<span data-ttu-id="70509-142">String collection</span><span class="sxs-lookup"><span data-stu-id="70509-142">String collection</span></span>| <span data-ttu-id="70509-143">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="70509-143">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="70509-144">Veja mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="70509-144">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="70509-145">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70509-145">Required.</span></span>|
|<span data-ttu-id="70509-146">description</span><span class="sxs-lookup"><span data-stu-id="70509-146">description</span></span>|<span data-ttu-id="70509-147">String</span><span class="sxs-lookup"><span data-stu-id="70509-147">String</span></span>| <span data-ttu-id="70509-148">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="70509-148">Description for this policy.</span></span>|
|<span data-ttu-id="70509-149">displayName</span><span class="sxs-lookup"><span data-stu-id="70509-149">displayName</span></span>|<span data-ttu-id="70509-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="70509-150">String</span></span>| <span data-ttu-id="70509-151">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="70509-151">Display name for this policy.</span></span> <span data-ttu-id="70509-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70509-152">Required.</span></span>|
|<span data-ttu-id="70509-153">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="70509-153">isOrganizationDefault</span></span>|<span data-ttu-id="70509-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="70509-154">Boolean</span></span>|<span data-ttu-id="70509-155">Ignore essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="70509-155">Ignore this property.</span></span> <span data-ttu-id="70509-156">A política de emissão de token só pode ser aplicada a entidades de serviço e não pode ser definida globalmente para a organização.</span><span class="sxs-lookup"><span data-stu-id="70509-156">The token-issuance policy can only be applied to service principals and can't be set globally for the organization.</span></span>|


### <a name="properties-of-a-token-issuance-policy-definition"></a><span data-ttu-id="70509-157">Propriedades de uma definição de política de emissão de token</span><span class="sxs-lookup"><span data-stu-id="70509-157">Properties of a token issuance policy definition</span></span>
<span data-ttu-id="70509-158">O formulário Propriedades o objeto JSON que representa uma política de emissão de tokens.</span><span class="sxs-lookup"><span data-stu-id="70509-158">The properties form the JSON object that represents a token issuance policy.</span></span> <span data-ttu-id="70509-159">Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** .</span><span class="sxs-lookup"><span data-stu-id="70509-159">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="70509-160">Veja a seguir um exemplo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="70509-160">The following is an example in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{ \"TokenIssuancePolicy\":{\"TokenResponseSigningPolicy\":\"TokenOnly\",\"SamlTokenVersion\":\"1.1\",\"SigningAlgorithm\":\"http://www.w3.org/2001/04/xmldsig-more#rsa-sha256\",\"Version\":1}}"
  ]
```


| <span data-ttu-id="70509-161">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70509-161">Property</span></span>     | <span data-ttu-id="70509-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="70509-162">Type</span></span>   |<span data-ttu-id="70509-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="70509-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70509-164">TokenResponseSigningPolicy</span><span class="sxs-lookup"><span data-stu-id="70509-164">TokenResponseSigningPolicy</span></span>|<span data-ttu-id="70509-165">String</span><span class="sxs-lookup"><span data-stu-id="70509-165">String</span></span>|<span data-ttu-id="70509-166">Representa as opções de assinatura de certificado disponíveis no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="70509-166">Represents the certificate signing options available in Azure AD.</span></span> <span data-ttu-id="70509-167">Os valores com suporte `ResponseOnly`são `TokenOnly`: `ResponseAndToken`,,.</span><span class="sxs-lookup"><span data-stu-id="70509-167">Supported values are: `ResponseOnly`, `TokenOnly`, `ResponseAndToken`.</span></span>  |
|<span data-ttu-id="70509-168">SamlTokenVersion</span><span class="sxs-lookup"><span data-stu-id="70509-168">SamlTokenVersion</span></span>|<span data-ttu-id="70509-169">String</span><span class="sxs-lookup"><span data-stu-id="70509-169">String</span></span>|<span data-ttu-id="70509-170">Versão do token SAML.</span><span class="sxs-lookup"><span data-stu-id="70509-170">Version of the SAML token.</span></span> <span data-ttu-id="70509-171">Os valores com suporte `1.1`são `2.0`:,.</span><span class="sxs-lookup"><span data-stu-id="70509-171">Supported values are: `1.1`, `2.0`.</span></span> |
|<span data-ttu-id="70509-172">SigningAlgorithm</span><span class="sxs-lookup"><span data-stu-id="70509-172">SigningAlgorithm</span></span>|<span data-ttu-id="70509-173">String</span><span class="sxs-lookup"><span data-stu-id="70509-173">String</span></span>|<span data-ttu-id="70509-174">Algoritmo de assinatura usado pelo Azure AD para assinar o token SAML.</span><span class="sxs-lookup"><span data-stu-id="70509-174">Signing algorithm use by Azure AD to sign the SAML token.</span></span> <span data-ttu-id="70509-175">Os valores com suporte `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256`são `http://www.w3.org/2000/09/xmldsig#rsa-sha1`:,.</span><span class="sxs-lookup"><span data-stu-id="70509-175">Supported values are: `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256`, `http://www.w3.org/2000/09/xmldsig#rsa-sha1`.</span></span>|
|<span data-ttu-id="70509-176">Versão</span><span class="sxs-lookup"><span data-stu-id="70509-176">Version</span></span>|<span data-ttu-id="70509-177">Inteiro</span><span class="sxs-lookup"><span data-stu-id="70509-177">Integer</span></span>|<span data-ttu-id="70509-178">Defina o valor 1.</span><span class="sxs-lookup"><span data-stu-id="70509-178">Set value of 1.</span></span> <span data-ttu-id="70509-179">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70509-179">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="70509-180">Relações</span><span class="sxs-lookup"><span data-stu-id="70509-180">Relationships</span></span>

| <span data-ttu-id="70509-181">Relação</span><span class="sxs-lookup"><span data-stu-id="70509-181">Relationship</span></span> | <span data-ttu-id="70509-182">Tipo</span><span class="sxs-lookup"><span data-stu-id="70509-182">Type</span></span>        | <span data-ttu-id="70509-183">Descrição</span><span class="sxs-lookup"><span data-stu-id="70509-183">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="70509-184">appliesTo</span><span class="sxs-lookup"><span data-stu-id="70509-184">appliesTo</span></span>|<span data-ttu-id="70509-185">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="70509-185">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="70509-186">A coleção [directoryobject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="70509-186">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="70509-187">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70509-187">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70509-188">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70509-188">JSON representation</span></span>

<span data-ttu-id="70509-189">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="70509-189">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
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
  "description": "tokenIssuancePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
