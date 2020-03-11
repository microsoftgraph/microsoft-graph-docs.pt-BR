---
title: tipo de recurso tokenIssuancePolicy
description: Representa a política para especificar as características dos tokens SAML emitidos pelo Azure AD.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0d88680ffd24133b0c5ddb3c9ac3dd3408a46dc2
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591786"
---
# <a name="tokenissuancepolicy-resource-type"></a>tipo de recurso tokenIssuancePolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a política para especificar as características dos tokens SAML emitidos pelo Azure AD. Você pode usar as políticas de emissão de tokens para:

- Definir opções de assinatura
- Definir algoritmo de assinatura
- Definir versão do token SAML

Herda de [stsPolicy](stsPolicy.md).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar tokenIssuancePolicy](../api/tokenissuancepolicy-post-tokenissuancepolicy.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | Criar um objeto tokenIssuancePolicy. |
| [Obter tokenIssuancePolicy](../api/tokenissuancepolicy-get.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | Ler propriedades e relações de um objeto tokenIssuancePolicy. |
| [Listar tokenIssuancePolicy](../api/tokenissuancepolicy-list.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | Ler propriedades e relações de objetos tokenIssuancePolicy. |
| [Atualizar tokenIssuancePolicy](../api/tokenissuancepolicy-update.md) | Nenhum | Atualizar um objeto tokenIssuancePolicy. |
| [Excluir tokenIssuancePolicy](../api/tokenissuancepolicy-delete.md) | Nenhum | Excluir um objeto tokenIssuancePolicy. |
| [Listar se aplica](../api/tokenissuancepolicy-list-appliesto.md) | Coleção [directoryObject](directoryobject.md) | Obtenha a lista de directoryObjects à qual essa política foi aplicada. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Identificador exclusivo da política. Somente leitura.|
|definir|Coleção de cadeias de caracteres| Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política. Veja mais detalhes sobre o esquema JSON para esta propriedade. Obrigatório.|
|description|String| Descrição da política.|
|displayName|Cadeia de caracteres| Nome para exibição dessa política. Obrigatório.|
|isOrganizationDefault|Booliano|Ignore essa propriedade. A política de emissão de token só pode ser aplicada a entidades de serviço e não pode ser definida globalmente para a organização.|


### <a name="properties-of-a-token-issuance-policy-definition"></a>Propriedades de uma definição de política de emissão de token
O formulário Propriedades o objeto JSON que representa uma política de emissão de tokens. Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** . Veja a seguir um exemplo no formato JSON:

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{ \"TokenIssuancePolicy\":{\"TokenResponseSigningPolicy\":\"TokenOnly\",\"SamlTokenVersion\":\"1.1\",\"SigningAlgorithm\":\"http://www.w3.org/2001/04/xmldsig-more#rsa-sha256\",\"Version\":1}}"
  ]
```


| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|TokenResponseSigningPolicy|String|Representa as opções de assinatura de certificado disponíveis no Azure AD. Os valores com suporte `ResponseOnly`são `TokenOnly`: `ResponseAndToken`,,.  |
|SamlTokenVersion|String|Versão do token SAML. Os valores com suporte `1.1`são `2.0`:,. |
|SigningAlgorithm|String|Algoritmo de assinatura usado pelo Azure AD para assinar o token SAML. Os valores com suporte `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256`são `http://www.w3.org/2000/09/xmldsig#rsa-sha1`:,.|
|Versão|Inteiro|Defina o valor 1. Obrigatório.|


## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|appliesTo|Coleção [directoryObject](directoryobject.md)| A coleção [directoryobject](directoryObject.md) à qual essa política foi aplicada. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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
