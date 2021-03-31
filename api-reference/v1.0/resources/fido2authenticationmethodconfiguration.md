---
title: tipo de recurso fido2AuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação FIDO2
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 00137618daf327793d7d60d8dadbe8ad89abc840
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468622"
---
# <a name="fido2authenticationmethodconfiguration-resource-type"></a>tipo de recurso fido2AuthenticationMethodConfiguration

Namespace: microsoft.graph

Representa uma política de métodos de autenticação FIDO2. As políticas de métodos de autenticação definem configurações e usuários ou grupos habilitados para usar o método de autenticação.


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Get](../api/fido2authenticationmethodconfiguration-get.md)|[fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md)|Leia as propriedades e as relações de um objeto fido2AuthenticationMethodConfiguration.|
|[Atualizar](../api/fido2authenticationmethodconfiguration-update.md)|[fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md)|Atualize as propriedades de um objeto fido2AuthenticationMethodConfiguration.|
|[Delete](../api/fido2authenticationmethodconfiguration-delete.md)|Nenhum|Reverte o objeto fido2AuthenticationMethodConfiguration para sua configuração padrão.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador de política do método de autenticação.|
|isAttestationEnforced|Booliano|Determina se o atestado deve ser imposto para o registro da chave de segurança FIDO2.|
|isSelfServiceRegistrationAllowed|Booliano|Determina se os usuários podem registrar novas chaves de segurança FIDO2.|
|keyRestrictions|[fido2KeyRestrictions](../resources/fido2keyrestrictions.md)|Controla se as restrições de chave são impostas às teclas de segurança FIDO2, permitindo ou desproteção de determinados tipos de chave, conforme definido pelo AAGUID (Authenticator Attestation GUID), um identificador que indica o tipo (por exemplo, make e model) do autenticador.|
|state|authenticationMethodState|Os valores possíveis são: `enabled`, `disabled`.|

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
