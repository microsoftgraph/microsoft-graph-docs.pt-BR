---
title: tipo de recurso claimsMappingPolicy
description: Representa uma política que pode controlar o tempo de vida de um token de acesso emitido pelo Azure Active Directory (Azure AD).
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8fe6ca32e606829f12400a03a70c9fb783f32f77
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234128"
---
# <a name="claimsmappingpolicy-resource-type"></a><span data-ttu-id="2bcc3-103">tipo de recurso claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="2bcc3-103">claimsMappingPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bcc3-104">Representa as políticas de mapeamento de declaração para protocolos WS-Alimentad, SAML, OAuth 2,0 e OpenID Connect, para tokens emitidos para um aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-104">Represents the claim-mapping policies for WS-Fed, SAML, OAuth 2.0, and OpenID Connect protocols, for tokens issued to a specific application.</span></span> <span data-ttu-id="2bcc3-105">Você pode usar políticas de mapeamento de declarações para:</span><span class="sxs-lookup"><span data-stu-id="2bcc3-105">You can use claims-mapping policies to:</span></span>

- <span data-ttu-id="2bcc3-106">Selecionar quais declarações são incluídas nos tokens</span><span class="sxs-lookup"><span data-stu-id="2bcc3-106">Select which claims are included in tokens</span></span>
- <span data-ttu-id="2bcc3-107">Criar tipos de declaração que ainda não existem</span><span class="sxs-lookup"><span data-stu-id="2bcc3-107">Create claim types that do not already exist</span></span>
- <span data-ttu-id="2bcc3-108">Escolha ou altere a fonte de dados emitidos em declarações específicas</span><span class="sxs-lookup"><span data-stu-id="2bcc3-108">Choose or change the source of data emitted in specific claims</span></span>  

<span data-ttu-id="2bcc3-109">Para obter mais detalhes de cenário e configuração, consulte [como: Personalizar declarações emitidas em tokens para um aplicativo específico em um locatário](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span><span class="sxs-lookup"><span data-stu-id="2bcc3-109">For more scenario and configuration details see [How to: Customize claims emitted in tokens for a specific app in a tenant](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span></span>

<span data-ttu-id="2bcc3-110">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2bcc3-110">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2bcc3-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="2bcc3-111">Methods</span></span>

| <span data-ttu-id="2bcc3-112">Método</span><span class="sxs-lookup"><span data-stu-id="2bcc3-112">Method</span></span>       | <span data-ttu-id="2bcc3-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2bcc3-113">Return Type</span></span> | <span data-ttu-id="2bcc3-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bcc3-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2bcc3-115">Criar claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="2bcc3-115">Create claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-post-claimsmappingpolicies.md) | [<span data-ttu-id="2bcc3-116">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="2bcc3-116">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="2bcc3-117">Criar um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-117">Create a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="2bcc3-118">Obter claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="2bcc3-118">Get claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-get.md) | [<span data-ttu-id="2bcc3-119">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="2bcc3-119">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="2bcc3-120">Ler propriedades e relações de um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-120">Read properties and relationships of a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="2bcc3-121">Listar claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="2bcc3-121">List claimsMappingPolicies</span></span>](../api/claimsmappingpolicy-list.md) | [<span data-ttu-id="2bcc3-122">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="2bcc3-122">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="2bcc3-123">Ler propriedades e relações de objetos claimsMappingPolicies.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-123">Read properties and relationships of claimsMappingPolicies objects.</span></span> |
| [<span data-ttu-id="2bcc3-124">Atualizar claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="2bcc3-124">Update claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-update.md) | <span data-ttu-id="2bcc3-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="2bcc3-125">None</span></span> | <span data-ttu-id="2bcc3-126">Atualizar um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-126">Update a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="2bcc3-127">Excluir claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="2bcc3-127">Delete claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-delete.md) | <span data-ttu-id="2bcc3-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="2bcc3-128">None</span></span> | <span data-ttu-id="2bcc3-129">Excluir um objeto claimsMappingPolicy.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-129">Delete a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="2bcc3-130">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="2bcc3-130">List appliesTo</span></span>](../api/claimsmappingpolicy-list-appliesto.md) | <span data-ttu-id="2bcc3-131">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="2bcc3-131">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="2bcc3-132">Obtenha a lista de directoryObjects à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-132">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="2bcc3-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2bcc3-133">Properties</span></span>

| <span data-ttu-id="2bcc3-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2bcc3-134">Property</span></span>     | <span data-ttu-id="2bcc3-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bcc3-135">Type</span></span>        | <span data-ttu-id="2bcc3-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bcc3-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2bcc3-137">id</span><span class="sxs-lookup"><span data-stu-id="2bcc3-137">id</span></span>|<span data-ttu-id="2bcc3-138">String</span><span class="sxs-lookup"><span data-stu-id="2bcc3-138">String</span></span>| <span data-ttu-id="2bcc3-139">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-139">Unique identifier for this policy.</span></span> <span data-ttu-id="2bcc3-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-140">Read-only.</span></span>|
|<span data-ttu-id="2bcc3-141">definir</span><span class="sxs-lookup"><span data-stu-id="2bcc3-141">definition</span></span>|<span data-ttu-id="2bcc3-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bcc3-142">String collection</span></span>| <span data-ttu-id="2bcc3-143">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-143">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="2bcc3-144">Veja mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-144">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="2bcc3-145">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-145">Required.</span></span>|
|<span data-ttu-id="2bcc3-146">description</span><span class="sxs-lookup"><span data-stu-id="2bcc3-146">description</span></span>|<span data-ttu-id="2bcc3-147">String</span><span class="sxs-lookup"><span data-stu-id="2bcc3-147">String</span></span>| <span data-ttu-id="2bcc3-148">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-148">Description for this policy.</span></span>|
|<span data-ttu-id="2bcc3-149">displayName</span><span class="sxs-lookup"><span data-stu-id="2bcc3-149">displayName</span></span>|<span data-ttu-id="2bcc3-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bcc3-150">String</span></span>| <span data-ttu-id="2bcc3-151">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-151">Display name for this policy.</span></span> <span data-ttu-id="2bcc3-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-152">Required.</span></span>|
|<span data-ttu-id="2bcc3-153">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="2bcc3-153">isOrganizationDefault</span></span>|<span data-ttu-id="2bcc3-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="2bcc3-154">Boolean</span></span>|<span data-ttu-id="2bcc3-155">Ignore essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-155">Ignore this property.</span></span> <span data-ttu-id="2bcc3-156">A política de mapeamento de declarações só pode ser aplicada a entidades de serviço e não pode ser definida globalmente para a organização.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-156">The claims-mapping policy can only be applied to service principals and can't be set globally for the organization.</span></span>|

### <a name="properties-of-a-claims-mapping-policy-definition"></a><span data-ttu-id="2bcc3-157">Propriedades de uma definição de política de mapeamento de declarações</span><span class="sxs-lookup"><span data-stu-id="2bcc3-157">Properties of a claims-mapping policy definition</span></span>

<span data-ttu-id="2bcc3-158">As propriedades abaixo formam o objeto JSON que representa uma política de mapeamento de declarações.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-158">The properties below form the JSON object that represents a claims-mapping policy.</span></span> <span data-ttu-id="2bcc3-159">Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** .</span><span class="sxs-lookup"><span data-stu-id="2bcc3-159">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="2bcc3-160">Alguns exemplos de definição são mostrados abaixo:</span><span class="sxs-lookup"><span data-stu-id="2bcc3-160">A few definition examples are shown below:</span></span>

#### <a name="example-definition-to-include-the-employeeid-and-tenantcountry-as-claims-in-tokens"></a><span data-ttu-id="2bcc3-161">Exemplo: **definição** para incluir o EmployeeID e TenantCountry como declarações em tokens</span><span class="sxs-lookup"><span data-stu-id="2bcc3-161">Example: **definition** to include the EmployeeID and TenantCountry as claims in tokens</span></span>
<!-- {
  "blockType": "ignored"
}-->
``` json
{
  "definition": [
    "{\"ClaimsMappingPolicy\":{
      \"Version\":1,
      \"IncludeBasicClaimSet\":\"true\", 
      \"ClaimsSchema\": [
        {\"Source\":\"user\",\"ID\":\"employeeid\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/name\",\"JwtClaimType\":\"name\"},{\"Source\":\"company\",\"ID\":\"tenantcountry\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/country\",\"JwtClaimType\":\"country\"}
        ]
      }
    }"
  ]
}
```

#### <a name="example-definition-that-uses-a-claims-transformation"></a><span data-ttu-id="2bcc3-162">Exemplo: **definição** que usa uma transformação de declarações</span><span class="sxs-lookup"><span data-stu-id="2bcc3-162">Example: **definition** that uses a claims transformation</span></span>
<!-- {
  "blockType": "ignored"
}-->
``` json
{
  "definition": [
    "{\"ClaimsMappingPolicy\":{
      \"Version\":1,
      \"IncludeBasicClaimSet\":\"true\", 
      \"ClaimsSchema\":[
        {\"Source\":\"user\",\"ID\":\"extensionattribute1\"},{\"Source\":\"transformation\",\"ID\":\"DataJoin\",\"TransformationId\":\"JoinTheData\",\"JwtClaimType\":\"JoinedData\"}
        ],
      \"ClaimsTransformation\":[
        {\"ID\":\"JoinTheData\",\"TransformationMethod\":\"Join\",\"InputClaims\":[{\"ClaimTypeReferenceId\":\"extensionattribute1\",\"TransformationClaimType\":\"string1\"}], \"InputParameters\": [{\"ID\":\"string2\",\"Value\":\"sandbox\"},{\"ID\":\"separator\",\"Value\":\".\"}],\"OutputClaims\":[{\"ClaimTypeReferenceId\":\"DataJoin\",\"TransformationClaimType\":\"outputClaim\"}]}
        ]
      }
    }"
  ]
}
```

| <span data-ttu-id="2bcc3-163">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2bcc3-163">Property</span></span>     | <span data-ttu-id="2bcc3-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bcc3-164">Type</span></span>   |<span data-ttu-id="2bcc3-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bcc3-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2bcc3-166">Versão</span><span class="sxs-lookup"><span data-stu-id="2bcc3-166">Version</span></span>|<span data-ttu-id="2bcc3-167">Inteiro</span><span class="sxs-lookup"><span data-stu-id="2bcc3-167">Integer</span></span>|<span data-ttu-id="2bcc3-168">Defina o valor 1.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-168">Set value of 1.</span></span> <span data-ttu-id="2bcc3-169">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-169">Required.</span></span>|
|<span data-ttu-id="2bcc3-170">IncludeBasicClaimSet</span><span class="sxs-lookup"><span data-stu-id="2bcc3-170">IncludeBasicClaimSet</span></span>|<span data-ttu-id="2bcc3-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="2bcc3-171">Boolean</span></span>|<span data-ttu-id="2bcc3-172">Se for definido como true, todas as declarações no conjunto de declarações básicas serão emitidas em tokens afetados pela política.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-172">If set to true, all claims in the basic claim set are emitted in tokens affected by the policy.</span></span> <span data-ttu-id="2bcc3-173">Se definido como false, as declarações no conjunto de declarações básicas não estão nos tokens, a menos que sejam individualmente adicionadas à propriedade ClaimsSchema da mesma política.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-173">If set to false, claims in the basic claim set are not in the tokens, unless they are individually added in the ClaimsSchema property of the same policy.</span></span>|
|<span data-ttu-id="2bcc3-174">ClaimsSchema</span><span class="sxs-lookup"><span data-stu-id="2bcc3-174">ClaimsSchema</span></span>|<span data-ttu-id="2bcc3-175">Objeto JSON</span><span class="sxs-lookup"><span data-stu-id="2bcc3-175">JSON object</span></span>|<span data-ttu-id="2bcc3-176">Define quais declarações estão presentes nos tokens afetados pela política, além do conjunto de declarações básico e o conjunto de declarações principal.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-176">Defines which claims are present in the tokens affected by the policy, in addition to the basic claim set and the core claim set.</span></span> <span data-ttu-id="2bcc3-177">Para cada entrada de esquema de declaração definida nessa propriedade, determinadas informações são necessárias.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-177">For each claim schema entry defined in this property, certain information is required.</span></span> <span data-ttu-id="2bcc3-178">Especifique onde os dados vêm vindo (par de valor ou código-fonte/ID) e quais declarações os dados são emitidos como (tipo de declaração).</span><span class="sxs-lookup"><span data-stu-id="2bcc3-178">Specify where the data is coming from (Value or Source/ID pair), and which claim the data is emitted as (Claim Type).</span></span> <span data-ttu-id="2bcc3-179">Mais detalhes estão disponíveis na [definição ClaimsSchema](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span><span class="sxs-lookup"><span data-stu-id="2bcc3-179">Further details are available in the [ClaimsSchema definition](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span></span>|
|<span data-ttu-id="2bcc3-180">ClaimsTransformation</span><span class="sxs-lookup"><span data-stu-id="2bcc3-180">ClaimsTransformation</span></span>|<span data-ttu-id="2bcc3-181">Objeto JSON</span><span class="sxs-lookup"><span data-stu-id="2bcc3-181">JSON object</span></span>| <span data-ttu-id="2bcc3-182">Define transformações comuns que podem ser aplicadas aos dados de origem, para gerar os dados de saída para declarações especificadas no ClaimsSchema.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-182">Defines common transformations that can be applied to source data, to generate the output data for claims specified in the ClaimsSchema.</span></span> <span data-ttu-id="2bcc3-183">Mais detalhes estão disponíveis na [definição ClaimsTransformation](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span><span class="sxs-lookup"><span data-stu-id="2bcc3-183">Further details are available in the [ClaimsTransformation definition](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span></span>|


## <a name="relationships"></a><span data-ttu-id="2bcc3-184">Relações</span><span class="sxs-lookup"><span data-stu-id="2bcc3-184">Relationships</span></span>

| <span data-ttu-id="2bcc3-185">Relação</span><span class="sxs-lookup"><span data-stu-id="2bcc3-185">Relationship</span></span> | <span data-ttu-id="2bcc3-186">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bcc3-186">Type</span></span>        | <span data-ttu-id="2bcc3-187">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bcc3-187">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2bcc3-188">appliesTo</span><span class="sxs-lookup"><span data-stu-id="2bcc3-188">appliesTo</span></span>|<span data-ttu-id="2bcc3-189">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="2bcc3-189">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="2bcc3-190">A coleção [directoryobject](directoryObject.md) à qual essa política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-190">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="2bcc3-191">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-191">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2bcc3-192">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2bcc3-192">JSON representation</span></span>

<span data-ttu-id="2bcc3-193">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2bcc3-193">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.claimsMappingPolicy",
  "baseType": "microsoft.graph.stsPolicy",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": false,
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "claimsMappingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->