---
title: Tipo de recurso temporaryAccessPassAuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação de Passagem de Acesso Temporário que define as definições de configuração e usuários ou grupos que estão habilitados para usar o método de autenticação.
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: fbcaa5a1d941a29a12a54699021a7e6ee1b25c41
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094065"
---
# <a name="temporaryaccesspassauthenticationmethodconfiguration-resource-type"></a>Tipo de recurso temporaryAccessPassAuthenticationMethodConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política de métodos de autenticação de Passagem de Acesso Temporário que define as definições de configuração e usuários ou grupos que estão habilitados para usar o método de autenticação de Passagem de Acesso [Temporário](temporaryaccesspassauthenticationmethod.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Get](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|Leia as propriedades e as relações de um **objeto temporaryAccessPassAuthenticationMethodConfiguration** .|
|[Atualizar](../api/temporaryaccesspassauthenticationmethodconfiguration-update.md)|Nenhum(a)|Atualize as propriedades de **um objeto temporaryAccessPassAuthenticationMethodConfiguration** .|
|[Excluir](../api/temporaryaccesspassauthenticationmethodconfiguration-delete.md)|Nenhum|Reverte **o objeto temporaryAccessPassAuthenticationMethodConfiguration** para sua configuração padrão.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|defaultLength|Int|Comprimento padrão em caracteres de um objeto De passagem de acesso temporário. Deve ter entre 8 e 48 caracteres.|
|defaultLifetimeInMinutes|Int|Tempo de vida padrão em minutos para uma Passagem de Acesso Temporária. O valor pode ser qualquer inteiro entre **minimumLifetimeInMinutes** e **maximumLifetimeInMinutes**.|
|id|Cadeia de caracteres|O identificador da política de método de autenticação. Herdado da [entidade](entity.md).|
|isUsableOnce|Booliano   |Se `true`, todas as passagens no locatário serão restritas ao uso único. Se `false`, passa o locatário pode ser criado para ser um uso único ou reutilizável.|
|minimumLifetimeInMinutes|Int|Tempo de vida mínimo em minutos para qualquer Passagem de Acesso Temporária criada no locatário. O valor pode estar entre 10 e 43200 minutos (equivalente a 30 dias).|
|maximumLifetimeInMinutes|Int|Tempo de vida máximo em minutos para qualquer Passagem de Acesso Temporária criada no locatário. O valor pode estar entre 10 e 43200 minutos (equivalente a 30 dias).|
|estado|authenticationMethodState|Se o método De passagem de acesso temporário está habilitado no locatário. Os valores possíveis são: `enabled` e `disabled`. Herdado [de authenticationMethodConfiguration](authenticationmethodconfiguration.md). |

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|includeTargets|[Coleção authenticationMethodTarget](../resources/authenticationmethodtarget.md)|Uma coleção de usuários ou grupos que estão habilitados para usar o método de autenticação.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "defaultLifetimeInMinutes": "Integer",
  "defaultLength": "Integer",
  "minimumLifetimeInMinutes": "Integer",
  "maximumLifetimeInMinutes": "Integer",
  "isUsableOnce": "Boolean",
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
