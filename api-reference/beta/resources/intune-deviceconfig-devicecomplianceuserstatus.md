---
title: Tipo de recurso deviceComplianceUserStatus
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b23a1b85696cb84d516cf284e46a9845be741be5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42793286"
---
# <a name="devicecomplianceuserstatus-resource-type"></a>Tipo de recurso deviceComplianceUserStatus

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

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



