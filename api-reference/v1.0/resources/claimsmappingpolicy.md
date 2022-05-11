---
title: Tipo de recurso claimsMappingPolicy
description: Representa as políticas de mapeamento de declaração para protocolos WS-Fed, SAML, OAuth 2.0 e OpenID Conexão, para tokens emitidos para um aplicativo específico.
ms.localizationpriority: medium
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b29c1c6bfd9fa3ac92b682e4a902aeda328230c0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315220"
---
# <a name="claimsmappingpolicy-resource-type"></a>Tipo de recurso claimsMappingPolicy

Namespace: microsoft.graph

Representa as políticas de mapeamento de declaração para protocolos WS-Fed, SAML, OAuth 2.0 e OpenID Conexão, para tokens emitidos para um aplicativo específico. Você pode usar políticas de mapeamento de declarações para:

- Selecionar quais declarações estão incluídas em tokens
- Criar tipos de declaração que ainda não existem
- Escolher ou alterar a fonte de dados emitidos em declarações específicas  

O número de declarações e transformações que podem ser adicionadas a uma política de mapeamento de declarações é limitado para reduzir o tamanho do token. Todas as entradas ou transformações de esquema de declarações que forem encontradas depois que o limite for atingido serão ignoradas e incluídas no token emitido. Para obter mais informações sobre os limites, consulte [Propriedades de uma definição de política de mapeamento de declarações](#properties-of-a-claims-mapping-policy-definition)

Para obter mais detalhes de cenário e configuração, consulte o tipo de política de mapeamento de declarações e como [personalizar declarações emitidas em tokens para um aplicativo específico em um locatário](/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).[](/azure/active-directory/develop/reference-claims-mapping-policy-type)

Herda de [stsPolicy](stsPolicy.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar claimsMappingPolicy](../api/claimsmappingpolicy-post-claimsmappingpolicies.md) | [claimsMappingPolicy](claimsmappingpolicy.md) | Crie um objeto claimsMappingPolicy. |
| [Obter claimsMappingPolicy](../api/claimsmappingpolicy-get.md) | [claimsMappingPolicy](claimsmappingpolicy.md) | Ler propriedades e relações de um objeto claimsMappingPolicy. |
| [Listar claimsMappingPolicies](../api/claimsmappingpolicy-list.md) | [claimsMappingPolicy](claimsmappingpolicy.md) | Ler propriedades e relações de objetos claimsMappingPolicies. |
| [Atualizar claimsMappingPolicy](../api/claimsmappingpolicy-update.md) | Nenhum | Atualize um objeto claimsMappingPolicy. |
| [Excluir claimsMappingPolicy](../api/claimsmappingpolicy-delete.md) | Nenhum | Exclua um objeto claimsMappingPolicy. |
| **Objetos de diretório** |  |  |
| [Lista appliesTo](../api/claimsmappingpolicy-list-appliesto.md) | Coleção [directoryObject](directoryobject.md) | Obtenha a lista de directoryObjects aos qual essa política foi aplicada. |
| [Atribuir claimsMappingPolicy](../api/serviceprincipal-post-claimsmappingpolicies.md) | Nenhum | Atribua um claimsMappingPolicy a um [objeto servicePrincipal](serviceprincipal.md) . |
| [Listar claimsMappingPolicy atribuído](../api/serviceprincipal-list-claimsmappingpolicies.md) | Conjunto [claimsMappingPolicy](claimsmappingpolicy.md) | Liste os objetos claimsMappingPolicy atribuídos a um [objeto servicePrincipal](serviceprincipal.md) . |
| [Remover claimsMappingPolicy](../api/serviceprincipal-delete-claimsmappingpolicies.md) | Nenhum | Remova um claimsMappingPolicy de um [objeto servicePrincipal](serviceprincipal.md) . |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres| Identificador exclusivo para esta política. Somente leitura.|
|Definição|Coleção de cadeias de caracteres| Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política. Consulte [Propriedades de uma definição de política de mapeamento de declarações](#properties-of-a-claims-mapping-policy-definition) para obter mais detalhes sobre o esquema JSON para essa propriedade. Obrigatório.|
|description|String| Descrição dessa política.|
|displayName|Cadeia de caracteres| Nome de exibição para esta política. Obrigatório.|
|isOrganizationDefault|Booliano|Ignore essa propriedade. A política de mapeamento de declarações só pode ser aplicada a entidades de serviço e não pode ser definida globalmente para a organização.|

### <a name="properties-of-a-claims-mapping-policy-definition"></a>Propriedades de uma definição de política de mapeamento de declarações

As propriedades abaixo formam o objeto JSON que representa uma política de mapeamento de declarações. Esse objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas escapadas** para ser inserido na propriedade **de definição** . Alguns exemplos de definição são mostrados abaixo:

#### <a name="example-definition-to-include-the-employeeid-and-tenantcountry-as-claims-in-tokens"></a>Exemplo: **definição** para incluir EmployeeID e TenantCountry como declarações em tokens
<!-- {
  "blockType": "ignored"
}-->
``` json
{
    "definition": [
        "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\",\"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"employeeid\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/name\",\"JwtClaimType\":\"name\"},{\"Source\":\"company\",\"ID\":\"tenantcountry\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/country\",\"JwtClaimType\":\"country\"}]}}"
    ],
    "displayName": "Test1234"
}
```

#### <a name="example-definition-that-uses-a-claims-transformation"></a>Exemplo: **definição** que usa uma transformação de declarações
<!-- {
  "blockType": "ignored"
}-->
``` json
{
    "definition": [
        "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\",\"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier\"},{\"Source\":\"user\",\"ID\":\"givenname\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname\"},{\"Source\":\"user\",\"ID\":\"displayname\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/name\"},{\"Source\":\"user\",\"ID\":\"surname\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname\"},{\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\":\"username\"}],\"ClaimsTransformation\":[{\"ID\":\"CreateTermsOfService\",\"TransformationMethod\":\"CreateStringClaim\",\"InputParameters\": [{\"ID\":\"value\",\"DataType\":\"string\", \"Value\":\"sandbox\"}],\"OutputClaims\":[{\"ClaimTypeReferenceId\":\"TOS\",\"TransformationClaimType\":\"createdClaim\"}]}]}}"
    ],
    "displayName": "Test1234"
}
```

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Versão|Inteiro|Defina o valor de 1. Obrigatório.|
|IncludeBasicClaimSet|Boolean|Se definido como `true`, todas as declarações no conjunto de declarações básicas serão emitidas em tokens afetados pela política. Se definido como `false`, as declarações no conjunto de declarações básicas não estão nos tokens, a menos que sejam adicionadas individualmente na propriedade ClaimsSchema da mesma política.|
|ClaimsSchema|Objeto JSON|Define quais declarações estão presentes nos tokens afetados pela política, além do conjunto de declarações básico e do conjunto de declarações principais. Para cada entrada de esquema de declaração definida nessa propriedade, determinadas informações são necessárias. Especifique de onde os dados são provenientes (par Valor ou Origem/ID) e qual declaração os dados são emitidos como (Tipo de Declaração). No máximo 50 declarações são incluídas no token por meio do objeto ClaimsSchema. Todas as entradas de esquema de declarações encontradas depois que o limite for atingido serão ignoradas e não aparecerão no token emitido. Mais detalhes estão disponíveis na [definição claimsSchema](/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).|
|ClaimsTransformation|Objeto JSON| Define transformações comuns que podem ser aplicadas aos dados de origem para gerar os dados de saída para declarações especificadas no ClaimsSchema. No máximo 50 transformações são incluídas no token por meio do objeto ClaimsTransformation. Todas as transformações encontradas depois que o limite for atingido serão ignoradas e não aparecerão no token emitido. Para obter mais informações sobre ClaimsTransformation e as funções com suporte, consulte [a transformação Declarações](/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).|


## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|Appliesto|Coleção [directoryObject](directoryobject.md)| A [coleção directoryObject](directoryObject.md) à qual essa política foi aplicada. Somente leitura.|

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
