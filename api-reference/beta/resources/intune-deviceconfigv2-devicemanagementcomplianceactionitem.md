---
title: Tipo de recurso deviceManagementComplianceActionItem
description: Ação agendada para a regra
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5d5bee49096634e52658c59a1e1e77df8c2fffed
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61334211"
---
# <a name="devicemanagementcomplianceactionitem-resource-type"></a>Tipo de recurso deviceManagementComplianceActionItem

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ação agendada para a regra

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementComplianceActionItems](../api/intune-deviceconfigv2-devicemanagementcomplianceactionitem-list.md)|[Coleção deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|Listar propriedades e relações dos [objetos deviceManagementComplianceActionItem.](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|
|[Obter deviceManagementComplianceActionItem](../api/intune-deviceconfigv2-devicemanagementcomplianceactionitem-get.md)|[deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|Leia propriedades e relações do [objeto deviceManagementComplianceActionItem.](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|
|[Criar deviceManagementComplianceActionItem](../api/intune-deviceconfigv2-devicemanagementcomplianceactionitem-create.md)|[deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|Crie um novo [objeto deviceManagementComplianceActionItem.](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|
|[Excluir deviceManagementComplianceActionItem](../api/intune-deviceconfigv2-devicemanagementcomplianceactionitem-delete.md)|Nenhum|Exclui um [deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md).|
|[Atualizar deviceManagementComplianceActionItem](../api/intune-deviceconfigv2-devicemanagementcomplianceactionitem-update.md)|[deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|Atualize as propriedades de [um objeto deviceManagementComplianceActionItem.](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave dessa configuração na política que a contém. Gerado automaticamente.|
|gracePeriodHours|Int32|Número de horas a aguardar até que a ação seja aplicada. Valores válidos de 0 a 8760|
|actionType|[deviceManagementComplianceActionType](../resources/intune-deviceconfigv2-devicemanagementcomplianceactiontype.md)|Que ação deve ser tomada. Os valores possíveis são: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.|
|notificationTemplateId|Cadeia de caracteres|Qual modelo de notificação de mensagem será usado|
|notificationMessageCCList|Coleção de cadeias de caracteres|Uma lista de IDs de grupo para especificar quem receberá uma cópia dessa mensagem de notificação. Essa coleção pode conter no máximo 100 elementos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementComplianceActionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementComplianceActionItem",
  "id": "String (identifier)",
  "gracePeriodHours": 1024,
  "actionType": "String",
  "notificationTemplateId": "String",
  "notificationMessageCCList": [
    "String"
  ]
}
```




