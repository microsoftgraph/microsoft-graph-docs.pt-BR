---
title: Tipo de recurso deviceComplianceUserStatus
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f71e4bb41c19ddb4b456ab42a4a723ab0e029163
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66733378"
---
# <a name="devicecomplianceuserstatus-resource-type"></a>Tipo de recurso deviceComplianceUserStatus

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceComplianceUserStatuses](../api/intune-deviceconfig-devicecomplianceuserstatus-list.md)|Conjunto [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|Listar propriedades e relações de objetos de [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).|
|[Obter deviceComplianceUserStatus](../api/intune-deviceconfig-devicecomplianceuserstatus-get.md)|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|Ler propriedades e relações de objetos de [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).|
|[Criar deviceComplianceUserStatus](../api/intune-deviceconfig-devicecomplianceuserstatus-create.md)|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|Criar um novo objeto de [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).|
|[Excluir deviceComplianceUserStatus](../api/intune-deviceconfig-devicecomplianceuserstatus-delete.md)|Nenhum|Excluir [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).|
|[Atualizar deviceComplianceUserStatus](../api/intune-deviceconfig-devicecomplianceuserstatus-update.md)|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|Atualizar as propriedades de um objeto de [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|userDisplayName|Cadeia de caracteres|Nome de usuário de DevicePolicyStatus.|
|devicesCount|Int32|Contagem de dispositivos para esse usuário.|
|status|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Status de conformidade do relatório de políticas. Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Data e hora da última modificação do relatório de políticas.|
|userPrincipalName|String|UserPrincipalName.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "devicesCount": 1024,
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```





