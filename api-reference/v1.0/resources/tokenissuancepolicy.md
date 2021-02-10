---
title: Tipo de recurso tokenIssuancePolicy
description: Representa a política para especificar as características dos tokens SAML emitidos pelo Azure AD.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a74664438d7a7201f331c4dca1105d523478e3ae
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154723"
---
# <a name="tokenissuancepolicy-resource-type"></a>Tipo de recurso tokenIssuancePolicy

Namespace: microsoft.graph



Representa a política para especificar as características dos tokens SAML emitidos pelo Azure AD. Você pode usar políticas de emissão de token para:

- Definir opções de assinatura
- Definir algoritmo de assinatura
- Definir a versão do token SAML

Herda de [stsPolicy](stsPolicy.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar tokenIssuancePolicy](../api/tokenissuancepolicy-list.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | Leia as propriedades e os relacionamentos dos objetos tokenIssuancePolicy. |
| [Criar tokenIssuancePolicy](../api/tokenissuancepolicy-post-tokenissuancepolicy.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | Crie um objeto tokenIssuancePolicy. |
| [Obter tokenIssuancePolicy](../api/tokenissuancepolicy-get.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | Ler propriedades e relações de um objeto tokenIssuancePolicy. |
| [Atualizar tokenIssuancePolicy](../api/tokenissuancepolicy-update.md) | Nenhum | Atualize um objeto tokenIssuancePolicy. |
| [Excluir tokenIssuancePolicy](../api/tokenissuancepolicy-delete.md) | Nenhum | Exclua um objeto tokenIssuancePolicy. |
| [Lista appliesTo](../api/tokenissuancepolicy-list-appliesto.md) | Coleção [directoryObject](directoryobject.md) | Obter a lista de directoryObjects aos qual essa política foi aplicada. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres| Identificador exclusivo desta política. Somente leitura.|
|definição|Coleção de cadeias de caracteres| Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política. Veja abaixo para obter mais detalhes sobre o esquema JSON para essa propriedade. Obrigatório.|
|description|Cadeia de caracteres| Descrição desta política.|
|displayName|Cadeia de caracteres| Nome para exibição desta política. Obrigatório.|
|isOrganizationDefault|Booliano|Ignore essa propriedade. A política de emissão de tokens só pode ser aplicada a entidades de serviço e não pode ser definida globalmente para a organização.|


### <a name="properties-of-a-token-issuance-policy-definition"></a>Propriedades de uma definição de política de emissão de token
As propriedades formam o objeto JSON que representa uma política de emissão de token. Esse objeto JSON deve ser **convertido em uma cadeia de caracteres** com aspas que não devem ser inseridas na propriedade de **definição.** Veja a seguir um exemplo no formato JSON:

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
|TokenResponseSigningPolicy|Cadeia de caracteres|Representa as opções de assinatura de certificado disponíveis no Azure AD. Os valores com suporte são: `ResponseOnly` , `TokenOnly` . `ResponseAndToken`  |
|SamlTokenVersion|Cadeia de caracteres|Versão do token SAML. Os valores com suporte são: `1.1` , `2.0` . |
|SigningAlgorithm|Cadeia de caracteres|Algoritmo de assinatura usado pelo Azure AD para assinar o token SAML. Os valores com suporte são: `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256` , `http://www.w3.org/2000/09/xmldsig#rsa-sha1` .|
|Versão|Inteiro|Valor definido de 1. Obrigatório.|


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

