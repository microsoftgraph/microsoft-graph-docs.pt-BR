---
title: Tipo de recurso temporaryAccessPassAuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação de Passagem de Acesso Temporário.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9edb4038180a96d6878fcaf6770728a1befbca19
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272587"
---
# <a name="temporaryaccesspassauthenticationmethodconfiguration-resource-type"></a>Tipo de recurso temporaryAccessPassAuthenticationMethodConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política de métodos de autenticação de Passagem de Acesso Temporário. A política de métodos de autenticação define as definições de configuração e os usuários ou grupos habilitados para usar o método de autenticação.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Get](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|Leia as propriedades e os relacionamentos de **um objeto temporaryaccesspassauthenticationmethodconfiguration.**|
|[Update](../api/temporaryaccesspassauthenticationmethodconfiguration-update.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|Atualizar as propriedades de **um objeto temporaryaccesspassauthenticationmethodconfiguration.**|
|[Delete](../api/temporaryaccesspassauthenticationmethodconfiguration-delete.md)|Nenhum|Reverte o **objeto temporaryaccesspassauthenticationmethodconfiguration** para sua configuração padrão.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador de política do método de autenticação.|
|minimumLifetimeInMinutes|Int|Tempo de vida mínimo em minutos para qualquer temporaryAccessPass criado no locatário. O valor pode estar entre 10 e 43.200 minutos (equivalente a 30 dias).|
|maximumLifetimeInMinutes|Int|Tempo de vida máximo em minutos para qualquer temporaryAccessPass criado no locatário. O valor pode estar entre 10 e 43.200 minutos (equivalente a 30 dias).|
|defaultLifetimeInMinutes|int|Tempo de vida padrão, em minutos, para um temporaryAccessPass. O valor pode estar entre minimumLifetimeInMinutes e maximumLifetimeInMinutes.|
|defaultLength|int|Comprimento padrão, em caracteres, de um temporaryAccessPass, entre 8 e 48 caracteres.|
|isUsableOnce|Booliano   |Se `true` , todas as passagens no locatário serão restritas ao uso único. Se , passa no locatário pode ser criado para ser uso único ou `false` uso de várias vezes.|
|estado|authenticationMethodState|Os valores possíveis são: `enabled`, `disabled`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|includeTargets|[Coleção authenticationMethodTarget](../resources/authenticationmethodtarget.md)|Uma coleção de usuários ou grupos que estão habilitados para usar o método de autenticação.|

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
