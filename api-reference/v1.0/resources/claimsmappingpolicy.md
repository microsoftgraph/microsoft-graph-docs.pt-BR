---
title: tipo de recurso claimsMappingPolicy
description: Representa as políticas de mapeamento de declaração para protocolos WS-Fed, SAML, OAuth 2.0 e OpenID Conexão, para tokens emitidos para um aplicativo específico.
localization_priority: Normal
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2ef027ac3729f85cc7f0e925067dd785eb10adfc86cea29435f02aecb6fc46b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189875"
---
# <a name="claimsmappingpolicy-resource-type"></a>tipo de recurso claimsMappingPolicy

Namespace: microsoft.graph

Representa as políticas de mapeamento de declaração para protocolos WS-Fed, SAML, OAuth 2.0 e OpenID Conexão, para tokens emitidos para um aplicativo específico. Você pode usar políticas de mapeamento de declarações para:

- Selecione quais declarações estão incluídas em tokens
- Criar tipos de declaração que ainda não existem
- Escolher ou alterar a fonte de dados emitidos em declarações específicas  

Para obter mais detalhes de cenário e configuração, consulte [How to: Customize claims emitted in tokens for a specific app in a tenant](/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).

Herda de [stsPolicy](stsPolicy.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar claimsMappingPolicy](../api/claimsmappingpolicy-post-claimsmappingpolicies.md) | [claimsMappingPolicy](claimsmappingpolicy.md) | Crie um objeto claimsMappingPolicy. |
| [Obter claimsMappingPolicy](../api/claimsmappingpolicy-get.md) | [claimsMappingPolicy](claimsmappingpolicy.md) | Leia propriedades e relações de um objeto claimsMappingPolicy. |
| [Listar claimsMappingPolicies](../api/claimsmappingpolicy-list.md) | [claimsMappingPolicy](claimsmappingpolicy.md) | Ler propriedades e relações de objetos claimsMappingPolicies. |
| [Update claimsMappingPolicy](../api/claimsmappingpolicy-update.md) | None | Atualize um objeto claimsMappingPolicy. |
| [Excluir claimsMappingPolicy](../api/claimsmappingpolicy-delete.md) | None | Exclua um objeto claimsMappingPolicy. |
| [Lista appliesTo](../api/claimsmappingpolicy-list-appliesto.md) | Coleção [directoryObject](directoryobject.md) | Obter a lista de directoryObjects aos qual essa política foi aplicada. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Identificador exclusivo dessa política. Apenas leitura.|
|definition|Coleção de cadeias de caracteres| Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política. Consulte abaixo para obter mais detalhes sobre o esquema JSON para esta propriedade. Obrigatório.|
|description|Cadeia de caracteres| Descrição dessa política.|
|displayName|Cadeia de caracteres| Nome de exibição para esta política. Obrigatório.|
|isOrganizationDefault|Booliano|Ignore essa propriedade. A política de mapeamento de declarações só pode ser aplicada a entidades de serviço e não pode ser definida globalmente para a organização.|

### <a name="properties-of-a-claims-mapping-policy-definition"></a>Propriedades de uma definição de política de mapeamento de declarações

As propriedades abaixo formam o objeto JSON que representa uma política de mapeamento de declarações. Esse objeto JSON deve ser **convertido em uma cadeia de caracteres com** aspas que escapam para serem inseridas na propriedade **definition.** Alguns exemplos de definição são mostrados abaixo:

#### <a name="example-definition-to-include-the-employeeid-and-tenantcountry-as-claims-in-tokens"></a>Exemplo: **definição** para incluir EmployeeID e TenantCountry como declarações em tokens
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

#### <a name="example-definition-that-uses-a-claims-transformation"></a>Exemplo: **definição** que usa uma transformação de declarações
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

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Versão|Inteiro|Definir o valor de 1. Obrigatório.|
|IncludeBasicClaimSet|Booliano|Se definido como true, todas as declarações no conjunto de declarações básico são emitidas em tokens afetados pela política. Se definido como false, as declarações no conjunto de declarações básicas não estão nos tokens, a menos que sejam adicionadas individualmente na propriedade ClaimsSchema da mesma política.|
|ClaimsSchema|Objeto JSON|Define quais declarações estão presentes nos tokens afetados pela política, além do conjunto de declarações básico e do conjunto de declarações principais. Para cada entrada de esquema de declaração definida nesta propriedade, determinadas informações são necessárias. Especifique de onde os dados estão vindo (par Valor ou Fonte/ID) e que dizem que os dados são emitidos como (Tipo de Declaração). Para obter mais informações, consulte [ClaimsSchema definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).|
|ClaimsTransformation|Objeto JSON| Define transformações comuns que podem ser aplicadas aos dados de origem, para gerar os dados de saída para declarações especificadas no ClaimsSchema. Para obter mais informações, consulte [ClaimsTransformation definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).|


## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|appliesTo|Coleção [directoryObject](directoryobject.md)| A [coleção directoryObject](directoryObject.md) à qual essa política foi aplicada. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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
