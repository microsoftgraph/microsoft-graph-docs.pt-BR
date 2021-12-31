---
title: Tipo de recurso accessPackageSubject
description: No gerenciamento de direitos do Azure AD, um assunto de uma atribuição de pacote de acesso.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d8c8a7bb8943f88657392f06ea78ec2ec502d436
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651439"
---
# <a name="accesspackagesubject-resource-type"></a>Tipo de recurso accessPackageSubject

Namespace: microsoft.graph


No gerenciamento de direitos do [Azure AD,](entitlementmanagement-overview.md)um assunto do pacote de acesso é um usuário, entidade de serviço ou outra entidade que pode ser configurada para solicitar ou ter um pacote de acesso atribuído.  Ele pode representar um solicitante de uma organização conectada que ainda não está no locatário.

## <a name="methods"></a>Métodos

Nenhum.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome de exibição do assunto.|
|email|Cadeia de caracteres|O endereço de email do assunto.|
|id|String|Somente leitura.|
|objectId|Cadeia de caracteres|O identificador de objeto do assunto. `null` se o assunto ainda não for um usuário no locatário.|
|onPremisesSecurityIdentifier|String|Uma representação de cadeia de caracteres do identificador de segurança da entidade, se conhecida, ou se o assunto `null` não tiver um identificador de segurança.|
|principalName|Cadeia de caracteres|O nome principal, se conhecido, do assunto.|
|subjectType|accessPackageSubjectType|O tipo de recurso do assunto. Os valores possíveis são: `notSpecified`, `user`, `servicePrincipal`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|connectedOrganization|[connectedOrganization](connectedorganization.md)|A organização conectada do assunto. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageSubject",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageSubject",
  "id": "String (identifier)",
  "objectId": "String",
  "onPremisesSecurityIdentifier": "String",
  "displayName": "String",
  "principalName": "String",
  "email": "String",
  "subjectType": "String"
}
```

