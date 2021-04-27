---
title: tipo de recurso temporaryAccessPassAuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação de Passagem de Acesso Temporário.
author: inbarckms
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 5cac99576931ff15636df6f69b548ecfb53c01f3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052541"
---
# <a name="temporaryaccesspassauthenticationmethodconfiguration-resource-type"></a>tipo de recurso temporaryAccessPassAuthenticationMethodConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política de métodos de autenticação de Passagem de Acesso Temporário. A política de métodos de autenticação define as configurações e usuários ou grupos habilitados para usar o método de autenticação.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Get](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|Leia as propriedades e as relações de **um objeto temporaryaccesspassauthenticationmethodconfiguration.**|
|[Atualizar](../api/temporaryaccesspassauthenticationmethodconfiguration-update.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|Atualize as propriedades de **um objeto temporaryaccesspassauthenticationmethodconfiguration.**|
|[Delete](../api/temporaryaccesspassauthenticationmethodconfiguration-delete.md)|Nenhuma|Reverte o **objeto temporaryaccesspassauthenticationmethodconfiguration** para sua configuração padrão.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador de política do método de autenticação.|
|minimumLifetimeInMinutes|Int|Tempo de vida mínimo em minutos para qualquer temporaryAccessPass criado no locatário. O valor pode estar entre 10 e 43200 minutos (equivalente a 30 dias).|
|maximumLifetimeInMinutes|Int|Vida máxima em minutos para qualquer temporaryAccessPass criado no locatário. O valor pode estar entre 10 e 43200 minutos (equivalente a 30 dias).|
|defaultLifetimeInMinutes|int|Tempo de vida padrão, em minutos, para um TemporaryAccessPass. O valor pode estar entre minimumLifetimeInMinutes e maximumLifetimeInMinutes.|
|defaultLength|int|Comprimento padrão, em caracteres, de um temporaryAccessPass, entre 8 e 48 caracteres.|
|isUsableOnce|Boolean   |Se `true` , todas as passagens no locatário serão restritas ao uso único. Se , o locatário pode ser criado para uso único ou `false` uso de várias vezes.|
|state|authenticationMethodState|Os valores possíveis são: `enabled`, `disabled`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|includeTargets|[coleção authenticationMethodTarget](../resources/authenticationmethodtarget.md)|Uma coleção de usuários ou grupos habilitados para usar o método de autenticação.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

``` json
{
  "@odata.type": "#microsoft.authMethodPolicy.temporaryAccessPassAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "defaultLifetimeInMinutes": "Integer",
  "defaultLength": "Integer",
  "minimumLifetimeInMinutes": "Integer",
  "maximumLifetimeInMinutes": "Integer",
  "isUsableOnce": "Boolean"
},
"includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
