---
title: Tipo de recurso temporaryAccessPassAuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação de Passagem de Acesso Temporário.
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 073e89cccf4f63760bcf7bcc79a28c4a0c6f7e58
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971200"
---
# <a name="temporaryaccesspassauthenticationmethodconfiguration-resource-type"></a>Tipo de recurso temporaryAccessPassAuthenticationMethodConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política de métodos de autenticação de Passagem de Acesso Temporário. A política de métodos de autenticação define as definições de configuração e os usuários ou grupos que estão habilitados para usar o método de autenticação.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Get](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|Leia as propriedades e as relações de um **objeto temporaryaccesspassauthenticationmethodconfiguration** .|
|[Atualizar](../api/temporaryaccesspassauthenticationmethodconfiguration-update.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|Atualize as propriedades de **um objeto temporaryaccesspassauthenticationmethodconfiguration** .|
|[Excluir](../api/temporaryaccesspassauthenticationmethodconfiguration-delete.md)|Nenhum|Reverte **o objeto temporaryaccesspassauthenticationmethodconfiguration** para sua configuração padrão.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador de política do método de autenticação.|
|minimumLifetimeInMinutes|Int|Tempo de vida mínimo em minutos para qualquer temporaryAccessPass criado no locatário. O valor pode estar entre 10 e 43200 minutos (equivalente a 30 dias).|
|maximumLifetimeInMinutes|Int|Tempo de vida máximo em minutos para qualquer temporaryAccessPass criado no locatário. O valor pode estar entre 10 e 43200 minutos (equivalente a 30 dias).|
|defaultLifetimeInMinutes|int|Tempo de vida padrão, em minutos, para um temporaryAccessPass. O valor pode estar entre minimumLifetimeInMinutes e maximumLifetimeInMinutes.|
|defaultLength|int|Comprimento padrão, em caracteres, de um temporaryAccessPass, entre 8 e 48 caracteres.|
|isUsableOnce|Booleano   |Se `true`, todas as passagens no locatário serão restritas ao uso único. Se `false`, as passagens no locatário podem ser criadas para uso único ou uso múltiplo.|
|estado|authenticationMethodState|Os valores possíveis são: `enabled`, `disabled`.|

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
  "isUsableOnce": "Boolean"
}
```
