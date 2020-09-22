---
title: tipo de recurso tokenIssuancePolicy
description: Representa a política para especificar as características dos tokens SAML emitidos pelo Azure AD.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: afba8ad5c1022156e68dbf27ad0e4199b573117b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090715"
---
# <a name="tokenissuancepolicy-resource-type"></a><span data-ttu-id="d7a23-103">tipo de recurso tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="d7a23-103">tokenIssuancePolicy resource type</span></span>

<span data-ttu-id="d7a23-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7a23-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="d7a23-105">Representa a política para especificar as características dos tokens SAML emitidos pelo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d7a23-105">Represents the policy to specify the characteristics of SAML tokens issued by Azure AD.</span></span> <span data-ttu-id="d7a23-106">Você pode usar as políticas de emissão de tokens para:</span><span class="sxs-lookup"><span data-stu-id="d7a23-106">You can use token-issuance policies to:</span></span>

- <span data-ttu-id="d7a23-107">Definir opções de assinatura</span><span class="sxs-lookup"><span data-stu-id="d7a23-107">Set signing options</span></span>
- <span data-ttu-id="d7a23-108">Definir algoritmo de assinatura</span><span class="sxs-lookup"><span data-stu-id="d7a23-108">Set signing algorithm</span></span>
- <span data-ttu-id="d7a23-109">Definir versão do token SAML</span><span class="sxs-lookup"><span data-stu-id="d7a23-109">Set SAML token version</span></span>

<span data-ttu-id="d7a23-110">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d7a23-110">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d7a23-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="d7a23-111">Methods</span></span>

| <span data-ttu-id="d7a23-112">Método</span><span class="sxs-lookup"><span data-stu-id="d7a23-112">Method</span></span>       | <span data-ttu-id="d7a23-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d7a23-113">Return Type</span></span> | <span data-ttu-id="d7a23-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7a23-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d7a23-115">Listar tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="d7a23-115">List tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-list.md) | [<span data-ttu-id="d7a23-116">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="d7a23-116">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="d7a23-117">Ler propriedades e relações de objetos tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="d7a23-117">Read properties and relationships of tokenIssuancePolicy objects.</span></span> |
| [<span data-ttu-id="d7a23-118">Criar tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="d7a23-118">Create tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-post-tokenissuancepolicy.md) | [<span data-ttu-id="d7a23-119">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="d7a23-119">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="d7a23-120">Criar um objeto tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="d7a23-120">Create a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="d7a23-121">Obter tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="d7a23-121">Get tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-get.md) | [<span data-ttu-id="d7a23-122">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="d7a23-122">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="d7a23-123">Ler propriedades e relações de um objeto tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="d7a23-123">Read properties and relationships of a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="d7a23-124">Atualizar tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="d7a23-124">Update tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-update.md) | <span data-ttu-id="d7a23-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d7a23-125">None</span></span> | <span data-ttu-id="d7a23-126">Atualizar um objeto tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="d7a23-126">Update a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="d7a23-127">Excluir tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="d7a23-127">Delete tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-delete.md) | <span data-ttu-id="d7a23-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d7a23-128">None</span></span> | <span data-ttu-id="d7a23-129">Excluir um objeto tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="d7a23-129">Delete a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="d7a23-130">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="d7a23-130">List appliesTo</span></span>](../api/tokenissuancepolicy-list-appliesto.md) | <span data-ttu-id="d7a23-131">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="d7a23-131">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="d7a23-132">Obtenha a lista de directoryObjects à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="d7a23-132">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="d7a23-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d7a23-133">Properties</span></span>

| <span data-ttu-id="d7a23-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7a23-134">Property</span></span>     | <span data-ttu-id="d7a23-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7a23-135">Type</span></span>        | <span data-ttu-id="d7a23-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7a23-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d7a23-137">id</span><span class="sxs-lookup"><span data-stu-id="d7a23-137">id</span></span>|<span data-ttu-id="d7a23-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7a23-138">String</span></span>| <span data-ttu-id="d7a23-139">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="d7a23-139">Unique identifier for this policy.</span></span> <span data-ttu-id="d7a23-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d7a23-140">Read-only.</span></span>|
|<span data-ttu-id="d7a23-141">definir</span><span class="sxs-lookup"><span data-stu-id="d7a23-141">definition</span></span>|<span data-ttu-id="d7a23-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d7a23-142">String collection</span></span>| <span data-ttu-id="d7a23-143">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="d7a23-143">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="d7a23-144">Veja mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="d7a23-144">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="d7a23-145">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7a23-145">Required.</span></span>|
|<span data-ttu-id="d7a23-146">description</span><span class="sxs-lookup"><span data-stu-id="d7a23-146">description</span></span>|<span data-ttu-id="d7a23-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7a23-147">String</span></span>| <span data-ttu-id="d7a23-148">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="d7a23-148">Description for this policy.</span></span>|
|<span data-ttu-id="d7a23-149">displayName</span><span class="sxs-lookup"><span data-stu-id="d7a23-149">displayName</span></span>|<span data-ttu-id="d7a23-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7a23-150">String</span></span>| <span data-ttu-id="d7a23-151">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="d7a23-151">Display name for this policy.</span></span> <span data-ttu-id="d7a23-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7a23-152">Required.</span></span>|
|<span data-ttu-id="d7a23-153">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="d7a23-153">isOrganizationDefault</span></span>|<span data-ttu-id="d7a23-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="d7a23-154">Boolean</span></span>|<span data-ttu-id="d7a23-155">Ignore essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="d7a23-155">Ignore this property.</span></span> <span data-ttu-id="d7a23-156">A política de emissão de token só pode ser aplicada a entidades de serviço e não pode ser definida globalmente para a organização.</span><span class="sxs-lookup"><span data-stu-id="d7a23-156">The token-issuance policy can only be applied to service principals and can't be set globally for the organization.</span></span>|


### <a name="properties-of-a-token-issuance-policy-definition"></a><span data-ttu-id="d7a23-157">Propriedades de uma definição de política de emissão de token</span><span class="sxs-lookup"><span data-stu-id="d7a23-157">Properties of a token issuance policy definition</span></span>
<span data-ttu-id="d7a23-158">O formulário Propriedades o objeto JSON que representa uma política de emissão de tokens.</span><span class="sxs-lookup"><span data-stu-id="d7a23-158">The properties form the JSON object that represents a token issuance policy.</span></span> <span data-ttu-id="d7a23-159">Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** .</span><span class="sxs-lookup"><span data-stu-id="d7a23-159">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="d7a23-160">Veja a seguir um exemplo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="d7a23-160">The following is an example in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{ \"TokenIssuancePolicy\":{\"TokenResponseSigningPolicy\":\"TokenOnly\",\"SamlTokenVersion\":\"1.1\",\"SigningAlgorithm\":\"http://www.w3.org/2001/04/xmldsig-more#rsa-sha256\",\"Version\":1}}"
  ]
```


| <span data-ttu-id="d7a23-161">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7a23-161">Property</span></span>     | <span data-ttu-id="d7a23-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7a23-162">Type</span></span>   |<span data-ttu-id="d7a23-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7a23-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7a23-164">TokenResponseSigningPolicy</span><span class="sxs-lookup"><span data-stu-id="d7a23-164">TokenResponseSigningPolicy</span></span>|<span data-ttu-id="d7a23-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7a23-165">String</span></span>|<span data-ttu-id="d7a23-166">Representa as opções de assinatura de certificado disponíveis no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d7a23-166">Represents the certificate signing options available in Azure AD.</span></span> <span data-ttu-id="d7a23-167">Os valores com suporte são: `ResponseOnly` , `TokenOnly` , `ResponseAndToken` .</span><span class="sxs-lookup"><span data-stu-id="d7a23-167">Supported values are: `ResponseOnly`, `TokenOnly`, `ResponseAndToken`.</span></span>  |
|<span data-ttu-id="d7a23-168">SamlTokenVersion</span><span class="sxs-lookup"><span data-stu-id="d7a23-168">SamlTokenVersion</span></span>|<span data-ttu-id="d7a23-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7a23-169">String</span></span>|<span data-ttu-id="d7a23-170">Versão do token SAML.</span><span class="sxs-lookup"><span data-stu-id="d7a23-170">Version of the SAML token.</span></span> <span data-ttu-id="d7a23-171">Os valores com suporte são: `1.1` , `2.0` .</span><span class="sxs-lookup"><span data-stu-id="d7a23-171">Supported values are: `1.1`, `2.0`.</span></span> |
|<span data-ttu-id="d7a23-172">SigningAlgorithm</span><span class="sxs-lookup"><span data-stu-id="d7a23-172">SigningAlgorithm</span></span>|<span data-ttu-id="d7a23-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7a23-173">String</span></span>|<span data-ttu-id="d7a23-174">Algoritmo de assinatura usado pelo Azure AD para assinar o token SAML.</span><span class="sxs-lookup"><span data-stu-id="d7a23-174">Signing algorithm use by Azure AD to sign the SAML token.</span></span> <span data-ttu-id="d7a23-175">Os valores com suporte são: `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256` , `http://www.w3.org/2000/09/xmldsig#rsa-sha1` .</span><span class="sxs-lookup"><span data-stu-id="d7a23-175">Supported values are: `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256`, `http://www.w3.org/2000/09/xmldsig#rsa-sha1`.</span></span>|
|<span data-ttu-id="d7a23-176">Versão</span><span class="sxs-lookup"><span data-stu-id="d7a23-176">Version</span></span>|<span data-ttu-id="d7a23-177">Inteiro</span><span class="sxs-lookup"><span data-stu-id="d7a23-177">Integer</span></span>|<span data-ttu-id="d7a23-178">Defina o valor 1.</span><span class="sxs-lookup"><span data-stu-id="d7a23-178">Set value of 1.</span></span> <span data-ttu-id="d7a23-179">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7a23-179">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="d7a23-180">Relações</span><span class="sxs-lookup"><span data-stu-id="d7a23-180">Relationships</span></span>

| <span data-ttu-id="d7a23-181">Relação</span><span class="sxs-lookup"><span data-stu-id="d7a23-181">Relationship</span></span> | <span data-ttu-id="d7a23-182">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7a23-182">Type</span></span>        | <span data-ttu-id="d7a23-183">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7a23-183">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d7a23-184">appliesTo</span><span class="sxs-lookup"><span data-stu-id="d7a23-184">appliesTo</span></span>|<span data-ttu-id="d7a23-185">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="d7a23-185">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="d7a23-186">A coleção [directoryobject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="d7a23-186">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="d7a23-187">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d7a23-187">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7a23-188">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d7a23-188">JSON representation</span></span>

<span data-ttu-id="d7a23-189">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d7a23-189">The following is a JSON representation of the resource.</span></span>

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

