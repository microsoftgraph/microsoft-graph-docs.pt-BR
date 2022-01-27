---
title: tipo de recurso authenticationMethodsPolicy
description: Define os métodos de autenticação e os usuários que têm permissão para usá-los para entrar e executar a autenticação multifato (MFA).
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: cea7a72bce9a87d199b71d7e5c91d8f91f9c8e51
ms.sourcegitcommit: de9df4bf6313b49afba74b6e9ef819907669c662
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2022
ms.locfileid: "62239096"
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
|id|Cadeia de caracteres|O identificador da política. Herdado da [entidade](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|A data e a hora da última atualização para a política. Apenas leitura.|
|policyVersion|Cadeia de Caracteres|A versão da política em uso. Apenas leitura.|
|registrationEnforcement|[registrationEnforcement](../resources/registrationenforcement.md)|Impor o registro no momento da inscrição. Essa propriedade pode ser usada para lembrar os usuários de configurar métodos de autenticação direcionados.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|authenticationMethodConfigurations|[coleção authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md)|Representa as configurações de cada método de autenticação. Expandida automaticamente no `GET /policies/authenticationMethodsPolicy`.|

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
  "registrationEnforcement": {
    "@odata.type": "microsoft.graph.registrationEnforcement"
  } 
}
```
