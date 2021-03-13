---
title: tipo de recurso smsAuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação de mensagem de texto.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c5a5e62e17e5b2e1cbc96ed96a44a0c483db981d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761034"
---
# <a name="smsauthenticationmethodconfiguration-resource-type"></a>tipo de recurso smsAuthenticationMethodConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política de métodos de autenticação de mensagem de texto. As políticas de métodos de autenticação definem configurações e usuários ou grupos habilitados para usar o método de autenticação.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Get](../api/smsauthenticationmethodconfiguration-get.md)|[smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md)|Leia as propriedades e as relações de um objeto smsAuthenticationMethodConfiguration.|
|[Update](../api/smsauthenticationmethodconfiguration-update.md)|[smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md)|Atualize as propriedades de um objeto smsAuthenticationMethodConfiguration.|
|[Delete](../api/smsauthenticationmethodconfiguration-delete.md)|Nenhum|Reverte o objeto smsAuthenticationMethodConfiguration para sua configuração padrão.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador de política do método de autenticação.|
|state|authenticationMethodState|Os valores possíveis são: `enabled`, `disabled`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|includeTargets|[coleção smsAuthenticationMethodTarget](../resources/smsauthenticationmethodtarget.md)|Uma coleção de usuários ou grupos habilitados para usar o método de autenticação.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.smsAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```

