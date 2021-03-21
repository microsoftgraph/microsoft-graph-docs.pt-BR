---
title: tipo de recurso fido2AuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação FIDO2
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7684b8b2c6601b4afdad25b3d3c32b7a6b68667d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964620"
---
# <a name="fido2authenticationmethodconfiguration-resource-type"></a>tipo de recurso fido2AuthenticationMethodConfiguration

Namespace: microsoft.graph

Representa uma política de métodos de autenticação FIDO2. As políticas de métodos de autenticação definem configurações e usuários ou grupos habilitados para usar o método de autenticação.


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Get](../api/fido2authenticationmethodconfiguration-get.md)|[fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md)|Leia as propriedades e as relações de um objeto fido2AuthenticationMethodConfiguration.|
|[Atualização](../api/fido2authenticationmethodconfiguration-update.md)|[fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md)|Atualize as propriedades de um objeto fido2AuthenticationMethodConfiguration.|
|[Delete](../api/fido2authenticationmethodconfiguration-delete.md)|Nenhum|Reverte o objeto fido2AuthenticationMethodConfiguration para sua configuração padrão.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador de política do método de autenticação.|
|isAttestationEnforced|Booliano|Determina se o atestado deve ser imposto para o registro da chave de segurança FIDO2.|
|isSelfServiceRegistrationAllowed|Booliano|Determina se os usuários podem registrar novas chaves de segurança FIDO2.|
|keyRestrictions|[fido2KeyRestrictions](../resources/fido2keyrestrictions.md)|Controla se as restrições de chave são impostas às teclas de segurança FIDO2, permitindo ou desproteção de determinados tipos de chave, conforme definido pelo AAGUID (Authenticator Attestation GUID), um identificador que indica o tipo (por exemplo, make e model) do autenticador.|
|estado|authenticationMethodState|Os valores possíveis são: `enabled`, `disabled`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|includeTargets|[coleção authenticationMethodTarget](../resources/authenticationmethodtarget.md)|Uma coleção de usuários ou grupos habilitados para usar o método de autenticação.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.fido2AuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "isSelfServiceRegistrationAllowed": "Boolean",
  "isAttestationEnforced": "Boolean",
  "keyRestrictions": {
    "@odata.type": "microsoft.graph.fido2KeyRestrictions"
  },
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
