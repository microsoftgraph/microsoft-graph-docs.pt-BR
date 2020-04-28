---
title: tipo de recurso tokenIssuancePolicy
description: Representa a política para especificar as características dos tokens SAML emitidos pelo Azure AD.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ecd776364fbdc3dcd0b4dbf59ff60c8e6624262b
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917366"
---
# <a name="tokenissuancepolicy-resource-type"></a><span data-ttu-id="84b8d-103">tipo de recurso tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="84b8d-103">tokenIssuancePolicy resource type</span></span>

<span data-ttu-id="84b8d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84b8d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84b8d-105">Representa a política para especificar as características dos tokens SAML emitidos pelo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="84b8d-105">Represents the policy to specify the characteristics of SAML tokens issued by Azure AD.</span></span> <span data-ttu-id="84b8d-106">Você pode usar as políticas de emissão de tokens para:</span><span class="sxs-lookup"><span data-stu-id="84b8d-106">You can use token-issuance policies to:</span></span>

- <span data-ttu-id="84b8d-107">Definir opções de assinatura</span><span class="sxs-lookup"><span data-stu-id="84b8d-107">Set signing options</span></span>
- <span data-ttu-id="84b8d-108">Definir algoritmo de assinatura</span><span class="sxs-lookup"><span data-stu-id="84b8d-108">Set signing algorithm</span></span>
- <span data-ttu-id="84b8d-109">Definir versão do token SAML</span><span class="sxs-lookup"><span data-stu-id="84b8d-109">Set SAML token version</span></span>

<span data-ttu-id="84b8d-110">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="84b8d-110">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="84b8d-111">Methods</span><span class="sxs-lookup"><span data-stu-id="84b8d-111">Methods</span></span>

| <span data-ttu-id="84b8d-112">Método</span><span class="sxs-lookup"><span data-stu-id="84b8d-112">Method</span></span>       | <span data-ttu-id="84b8d-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="84b8d-113">Return Type</span></span> | <span data-ttu-id="84b8d-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="84b8d-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="84b8d-115">Criar tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="84b8d-115">Create tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-post-tokenissuancepolicy.md) | [<span data-ttu-id="84b8d-116">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="84b8d-116">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="84b8d-117">Criar um objeto tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="84b8d-117">Create a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="84b8d-118">Obter tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="84b8d-118">Get tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-get.md) | [<span data-ttu-id="84b8d-119">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="84b8d-119">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="84b8d-120">Ler propriedades e relações de um objeto tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="84b8d-120">Read properties and relationships of a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="84b8d-121">Listar tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="84b8d-121">List tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-list.md) | [<span data-ttu-id="84b8d-122">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="84b8d-122">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="84b8d-123">Ler propriedades e relações de objetos tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="84b8d-123">Read properties and relationships of tokenIssuancePolicy objects.</span></span> |
| [<span data-ttu-id="84b8d-124">Atualizar tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="84b8d-124">Update tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-update.md) | <span data-ttu-id="84b8d-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="84b8d-125">None</span></span> | <span data-ttu-id="84b8d-126">Atualizar um objeto tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="84b8d-126">Update a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="84b8d-127">Excluir tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="84b8d-127">Delete tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-delete.md) | <span data-ttu-id="84b8d-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="84b8d-128">None</span></span> | <span data-ttu-id="84b8d-129">Excluir um objeto tokenIssuancePolicy.</span><span class="sxs-lookup"><span data-stu-id="84b8d-129">Delete a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="84b8d-130">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="84b8d-130">List appliesTo</span></span>](../api/tokenissuancepolicy-list-appliesto.md) | <span data-ttu-id="84b8d-131">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="84b8d-131">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="84b8d-132">Obtenha a lista de directoryObjects à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="84b8d-132">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="84b8d-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="84b8d-133">Properties</span></span>

| <span data-ttu-id="84b8d-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84b8d-134">Property</span></span>     | <span data-ttu-id="84b8d-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="84b8d-135">Type</span></span>        | <span data-ttu-id="84b8d-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="84b8d-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="84b8d-137">id</span><span class="sxs-lookup"><span data-stu-id="84b8d-137">id</span></span>|<span data-ttu-id="84b8d-138">String</span><span class="sxs-lookup"><span data-stu-id="84b8d-138">String</span></span>| <span data-ttu-id="84b8d-139">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="84b8d-139">Unique identifier for this policy.</span></span> <span data-ttu-id="84b8d-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="84b8d-140">Read-only.</span></span>|
|<span data-ttu-id="84b8d-141">definir</span><span class="sxs-lookup"><span data-stu-id="84b8d-141">definition</span></span>|<span data-ttu-id="84b8d-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="84b8d-142">String collection</span></span>| <span data-ttu-id="84b8d-143">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="84b8d-143">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="84b8d-144">Veja mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="84b8d-144">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="84b8d-145">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84b8d-145">Required.</span></span>|
|<span data-ttu-id="84b8d-146">description</span><span class="sxs-lookup"><span data-stu-id="84b8d-146">description</span></span>|<span data-ttu-id="84b8d-147">String</span><span class="sxs-lookup"><span data-stu-id="84b8d-147">String</span></span>| <span data-ttu-id="84b8d-148">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="84b8d-148">Description for this policy.</span></span>|
|<span data-ttu-id="84b8d-149">displayName</span><span class="sxs-lookup"><span data-stu-id="84b8d-149">displayName</span></span>|<span data-ttu-id="84b8d-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84b8d-150">String</span></span>| <span data-ttu-id="84b8d-151">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="84b8d-151">Display name for this policy.</span></span> <span data-ttu-id="84b8d-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84b8d-152">Required.</span></span>|
|<span data-ttu-id="84b8d-153">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="84b8d-153">isOrganizationDefault</span></span>|<span data-ttu-id="84b8d-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b8d-154">Boolean</span></span>|<span data-ttu-id="84b8d-155">Ignore essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="84b8d-155">Ignore this property.</span></span> <span data-ttu-id="84b8d-156">A política de emissão de token só pode ser aplicada a entidades de serviço e não pode ser definida globalmente para a organização.</span><span class="sxs-lookup"><span data-stu-id="84b8d-156">The token-issuance policy can only be applied to service principals and can't be set globally for the organization.</span></span>|


### <a name="properties-of-a-token-issuance-policy-definition"></a><span data-ttu-id="84b8d-157">Propriedades de uma definição de política de emissão de token</span><span class="sxs-lookup"><span data-stu-id="84b8d-157">Properties of a token issuance policy definition</span></span>
<span data-ttu-id="84b8d-158">O formulário Propriedades o objeto JSON que representa uma política de emissão de tokens.</span><span class="sxs-lookup"><span data-stu-id="84b8d-158">The properties form the JSON object that represents a token issuance policy.</span></span> <span data-ttu-id="84b8d-159">Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** .</span><span class="sxs-lookup"><span data-stu-id="84b8d-159">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="84b8d-160">Veja a seguir um exemplo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="84b8d-160">The following is an example in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{ \"TokenIssuancePolicy\":{\"TokenResponseSigningPolicy\":\"TokenOnly\",\"SamlTokenVersion\":\"1.1\",\"SigningAlgorithm\":\"http://www.w3.org/2001/04/xmldsig-more#rsa-sha256\",\"Version\":1}}"
  ]
```


| <span data-ttu-id="84b8d-161">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84b8d-161">Property</span></span>     | <span data-ttu-id="84b8d-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="84b8d-162">Type</span></span>   |<span data-ttu-id="84b8d-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="84b8d-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84b8d-164">TokenResponseSigningPolicy</span><span class="sxs-lookup"><span data-stu-id="84b8d-164">TokenResponseSigningPolicy</span></span>|<span data-ttu-id="84b8d-165">String</span><span class="sxs-lookup"><span data-stu-id="84b8d-165">String</span></span>|<span data-ttu-id="84b8d-166">Representa as opções de assinatura de certificado disponíveis no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="84b8d-166">Represents the certificate signing options available in Azure AD.</span></span> <span data-ttu-id="84b8d-167">Os valores com suporte `ResponseOnly`são `TokenOnly`: `ResponseAndToken`,,.</span><span class="sxs-lookup"><span data-stu-id="84b8d-167">Supported values are: `ResponseOnly`, `TokenOnly`, `ResponseAndToken`.</span></span>  |
|<span data-ttu-id="84b8d-168">SamlTokenVersion</span><span class="sxs-lookup"><span data-stu-id="84b8d-168">SamlTokenVersion</span></span>|<span data-ttu-id="84b8d-169">String</span><span class="sxs-lookup"><span data-stu-id="84b8d-169">String</span></span>|<span data-ttu-id="84b8d-170">Versão do token SAML.</span><span class="sxs-lookup"><span data-stu-id="84b8d-170">Version of the SAML token.</span></span> <span data-ttu-id="84b8d-171">Os valores com suporte `1.1`são `2.0`:,.</span><span class="sxs-lookup"><span data-stu-id="84b8d-171">Supported values are: `1.1`, `2.0`.</span></span> |
|<span data-ttu-id="84b8d-172">SigningAlgorithm</span><span class="sxs-lookup"><span data-stu-id="84b8d-172">SigningAlgorithm</span></span>|<span data-ttu-id="84b8d-173">String</span><span class="sxs-lookup"><span data-stu-id="84b8d-173">String</span></span>|<span data-ttu-id="84b8d-174">Algoritmo de assinatura usado pelo Azure AD para assinar o token SAML.</span><span class="sxs-lookup"><span data-stu-id="84b8d-174">Signing algorithm use by Azure AD to sign the SAML token.</span></span> <span data-ttu-id="84b8d-175">Os valores com suporte `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256`são `http://www.w3.org/2000/09/xmldsig#rsa-sha1`:,.</span><span class="sxs-lookup"><span data-stu-id="84b8d-175">Supported values are: `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256`, `http://www.w3.org/2000/09/xmldsig#rsa-sha1`.</span></span>|
|<span data-ttu-id="84b8d-176">Versão</span><span class="sxs-lookup"><span data-stu-id="84b8d-176">Version</span></span>|<span data-ttu-id="84b8d-177">Inteiro</span><span class="sxs-lookup"><span data-stu-id="84b8d-177">Integer</span></span>|<span data-ttu-id="84b8d-178">Defina o valor 1.</span><span class="sxs-lookup"><span data-stu-id="84b8d-178">Set value of 1.</span></span> <span data-ttu-id="84b8d-179">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84b8d-179">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="84b8d-180">Relações</span><span class="sxs-lookup"><span data-stu-id="84b8d-180">Relationships</span></span>

| <span data-ttu-id="84b8d-181">Relação</span><span class="sxs-lookup"><span data-stu-id="84b8d-181">Relationship</span></span> | <span data-ttu-id="84b8d-182">Tipo</span><span class="sxs-lookup"><span data-stu-id="84b8d-182">Type</span></span>        | <span data-ttu-id="84b8d-183">Descrição</span><span class="sxs-lookup"><span data-stu-id="84b8d-183">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="84b8d-184">appliesTo</span><span class="sxs-lookup"><span data-stu-id="84b8d-184">appliesTo</span></span>|<span data-ttu-id="84b8d-185">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="84b8d-185">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="84b8d-186">A coleção [directoryobject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="84b8d-186">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="84b8d-187">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="84b8d-187">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="84b8d-188">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="84b8d-188">JSON representation</span></span>

<span data-ttu-id="84b8d-189">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="84b8d-189">The following is a JSON representation of the resource.</span></span>

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
