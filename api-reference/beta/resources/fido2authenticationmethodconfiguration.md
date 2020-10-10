---
title: tipo de recurso fido2AuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação do FIDO2
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 62aa22fa22b70235f5221bc820cee5178b55b51b
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418171"
---
# <a name="fido2authenticationmethodconfiguration-resource-type"></a>tipo de recurso fido2AuthenticationMethodConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política de métodos de autenticação do FIDO2. Métodos de autenticação as políticas definem definições de configuração e usuários ou grupos que estão habilitados para usar o método de autenticação.


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Get](../api/fido2authenticationmethodconfiguration-get.md)|[fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md)|Leia as propriedades e os relacionamentos de um objeto fido2AuthenticationMethodConfiguration.|
|[Atualizar](../api/fido2authenticationmethodconfiguration-update.md)|[fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md)|Atualiza as propriedades de um objeto fido2AuthenticationMethodConfiguration.|
|[Excluir](../api/fido2authenticationmethodconfiguration-delete.md)|Nenhum|Reverte o objeto fido2AuthenticationMethodConfiguration para sua configuração padrão.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador de política de método de autenticação.|
|isAttestationEnforced|Boolean|Determina se o atestado deve ser aplicado para o registro da chave de segurança do FIDO2.|
|isSelfServiceRegistrationAllowed|Boolean|Determina se os usuários podem registrar novas chaves de segurança do FIDO2.|
|restrições de|[fido2KeyRestrictions](../resources/fido2keyrestrictions.md)|Controla se as restrições de chave são impostas nas chaves de segurança do FIDO2, permitindo ou não a permissão de certos tipos de chave, conforme definido pelo GUID de atestado de autenticador (AAGUID), um identificador que indica o tipo (por exemplo, Make e Model) do autenticador.|
|estado|authenticationMethodState|Os valores possíveis são: `enabled`, `disabled`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|includeTargets|coleção [authenticationMethodTarget](../resources/authenticationmethodtarget.md)|Uma coleção de usuários ou grupos que estão habilitados para usar o método de autenticação.|

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
