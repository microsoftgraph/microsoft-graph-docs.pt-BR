---
title: tipo de recurso authenticationMethodsPolicy
description: Define os métodos de autenticação e os usuários que têm permissão para usá-los para entrar e executar a autenticação multifato (MFA).
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9abab0af31a67465db9989b42186759b12f746bb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126958"
---
# <a name="authenticationmethodspolicy-resource-type"></a>tipo de recurso authenticationMethodsPolicy

Namespace: microsoft.graph

Define os métodos de autenticação e os usuários que têm permissão para usá-los para entrar e executar a autenticação multifato (MFA) no Azure Active Directory (Azure AD).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter authenticationMethodsPolicy](../api/authenticationmethodspolicy-get.md)|[authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md)|Leia as propriedades e as relações de um [objeto authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)|
|[Atualizar autenticaçãoMethodsPolicy](../api/authenticationmethodspolicy-update.md)|[authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md)|Atualize as propriedades de [um objeto authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|Cadeia de caracteres|Uma descrição da política. Somente leitura.|
|displayName|String|O nome da política. Somente leitura.|
|id|String|O identificador da política. Herdado da [entidade](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|A data e a hora da última atualização para a política. Somente leitura.|
|policyVersion|String|A versão da política em uso. Somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|authenticationMethodConfigurations|[coleção authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md)|Representa as configurações de cada método de autenticação.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodsPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "policyVersion": "String",
}
```
