---
title: Tipo de recurso tokenIssuancePolicy
description: Representa a política para especificar as características dos tokens SAML emitidos por Azure AD.
ms.localizationpriority: medium
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0ec511daf140c83887fad5c524c5c67084ba3810
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768284"
---
# <a name="tokenissuancepolicy-resource-type"></a>Tipo de recurso tokenIssuancePolicy

Namespace: microsoft.graph



Representa a política para especificar as características dos tokens SAML emitidos por Azure AD. Você pode usar políticas de emissão de token para:

- Definir opções de assinatura
- Definir algoritmo de assinatura
- Definir a versão do token SAML

Herda de [stsPolicy](stsPolicy.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar tokenIssuancePolicy](../api/tokenissuancepolicy-list.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | Ler propriedades e relações de objetos tokenIssuancePolicy. |
| [Criar tokenIssuancePolicy](../api/tokenissuancepolicy-post-tokenissuancepolicy.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | Crie um objeto tokenIssuancePolicy. |
| [Obter tokenIssuancePolicy](../api/tokenissuancepolicy-get.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | Ler propriedades e relações de um objeto tokenIssuancePolicy. |
| [Atualizar tokenIssuancePolicy](../api/tokenissuancepolicy-update.md) | Nenhum | Atualize um objeto tokenIssuancePolicy. |
| [Excluir tokenIssuancePolicy](../api/tokenissuancepolicy-delete.md) | Nenhum | Exclua um objeto tokenIssuancePolicy. |
| [Lista appliesTo](../api/tokenissuancepolicy-list-appliesto.md) | Coleção [directoryObject](directoryobject.md) | Obtenha a lista de directoryObjects aos qual essa política foi aplicada. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Identificador exclusivo para esta política. Somente leitura.|
|Definição|Conjunto de cadeias de caracteres| Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política. Consulte abaixo para obter mais detalhes sobre o esquema JSON para essa propriedade. Obrigatório.|
|description|String| Descrição dessa política.|
|displayName|String| Nome de exibição para esta política. Obrigatório.|
|isOrganizationDefault|Boolean|Ignore essa propriedade. A política de emissão de token só pode ser aplicada a entidades de serviço e não pode ser definida globalmente para a organização.|


### <a name="properties-of-a-token-issuance-policy-definition"></a>Propriedades de uma definição de política de emissão de token
As propriedades formam o objeto JSON que representa uma política de emissão de token. Esse objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas escapadas** para ser inserido na propriedade **de definição** . Este é um exemplo no formato JSON:

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{ \"TokenIssuancePolicy\":{\"TokenResponseSigningPolicy\":\"TokenOnly\",\"SamlTokenVersion\":\"1.1\",\"SigningAlgorithm\":\"http://www.w3.org/2001/04/xmldsig-more#rsa-sha256\",\"Version\":\"1\",\"EmitSAMLNameFormat\": \"true\"}}"
  ]
```


| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|TokenResponseSigningPolicy|String|Representa as opções de assinatura de certificado disponíveis Azure AD. Os valores com suporte são: `ResponseOnly`, `TokenOnly`, `ResponseAndToken`.  |
|SamlTokenVersion|String|Versão do token SAML. Os valores com suporte são: `1.1`, `2.0`. |
|SigningAlgorithm|String|O algoritmo de assinatura Azure AD para assinar o token SAML. Os valores com suporte são: `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256`, `http://www.w3.org/2000/09/xmldsig#rsa-sha1`.|
|Version|Inteiro|Defina o valor de 1. Obrigatório.|
| EmitSamlNameFormat | Boolean | Se selecionado, o Azure Active Directory adicionará um atributo adicional chamado "NameFormat" que descreve o formato do nome para declarações restritas, principais e opcionais para este aplicativo. [Saiba Mais](/azure/active-directory/develop/reference-claims-mapping-policy-type#claim-sets) |


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
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
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

