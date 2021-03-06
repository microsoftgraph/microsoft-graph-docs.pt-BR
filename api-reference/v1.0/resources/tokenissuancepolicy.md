---
title: Tipo de recurso tokenIssuancePolicy
description: Representa a política para especificar as características dos tokens SAML emitidos pelo Azure AD.
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 761e1d7e45f2d6a2cb11513cd3484a88a080888e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444319"
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
| [Token de listaIssuancePolicy](../api/tokenissuancepolicy-list.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | Leia propriedades e relações de objetos tokenIssuancePolicy. |
| [Criar tokenIssuancePolicy](../api/tokenissuancepolicy-post-tokenissuancepolicy.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | Crie um objeto tokenIssuancePolicy. |
| [Obter tokenIssuancePolicy](../api/tokenissuancepolicy-get.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | Leia propriedades e relações de um objeto tokenIssuancePolicy. |
| [Atualizar tokenIssuancePolicy](../api/tokenissuancepolicy-update.md) | Nenhum | Atualize um objeto tokenIssuancePolicy. |
| [Excluir tokenIssuancePolicy](../api/tokenissuancepolicy-delete.md) | Nenhum | Exclua um objeto tokenIssuancePolicy. |
| [Lista appliesTo](../api/tokenissuancepolicy-list-appliesto.md) | Coleção [directoryObject](directoryobject.md) | Obter a lista de directoryObjects aos qual essa política foi aplicada. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres| Identificador exclusivo dessa política. Somente leitura.|
|definition|Conjunto de cadeias de caracteres| Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política. Consulte abaixo para obter mais detalhes sobre o esquema JSON para esta propriedade. Obrigatório.|
|description|Cadeia de caracteres| Descrição dessa política.|
|displayName|Cadeia de caracteres| Nome de exibição para esta política. Obrigatório.|
|isOrganizationDefault|Boolean|Ignore essa propriedade. A política de emissão de token só pode ser aplicada a entidades de serviço e não pode ser definida globalmente para a organização.|


### <a name="properties-of-a-token-issuance-policy-definition"></a>Propriedades de uma definição de política de emissão de token
As propriedades formam o objeto JSON que representa uma política de emissão de token. Esse objeto JSON deve ser **convertido em uma cadeia de caracteres com** aspas que escapam para serem inseridas na propriedade **definition.** Veja a seguir um exemplo no formato JSON:

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
|TokenResponseSigningPolicy|Cadeia de caracteres|Representa as opções de assinatura de certificado disponíveis no Azure AD. Os valores suportados são: `ResponseOnly` , `TokenOnly` , `ResponseAndToken` .  |
|SamlTokenVersion|Cadeia de caracteres|Versão do token SAML. Os valores suportados são: `1.1` , `2.0` . |
|SigningAlgorithm|Cadeia de caracteres|O algoritmo de assinatura é usado pelo Azure AD para assinar o token SAML. Os valores suportados são: `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256` , `http://www.w3.org/2000/09/xmldsig#rsa-sha1` .|
|Versão|Inteiro|Definir o valor de 1. Obrigatório.|


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

