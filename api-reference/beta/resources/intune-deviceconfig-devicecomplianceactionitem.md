---
title: Tipo de recurso deviceComplianceActionItem
description: Configuração de ação agendada
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3962864aa220cd3231d69b0b069cc37342f192ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526729"
---
# <a name="devicecomplianceactionitem-resource-type"></a>Tipo de recurso deviceComplianceActionItem

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configuração de ação agendada

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceComplianceActionItems](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|Conjunto [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|Listar propriedades e relações de objetos de [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).|
|[Obter deviceComplianceActionItem](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|Ler propriedades e relações de objetos de [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).|
|[Criar deviceComplianceActionItem](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|Criar um novo objeto de [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).|
|[Excluir deviceComplianceActionItem](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|Nenhum|Excluir [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).|
|[Atualizar deviceComplianceActionItem](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|Atualizar as propriedades de um objeto de [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|gracePeriodHours|Int32|Número de horas a aguardar até que a ação seja aplicada. Valores válidos de 0 a 8760|
|actionType|[Enumeraçãodevicecomplianceactiontype](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|Qual ação executar. Os valores possíveis são: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.|
|notificationTemplateId|Cadeia de caracteres|Qual modelo de notificação de mensagem será usado|
|notificationMessageCCList|Coleção de cadeias de caracteres|Uma lista de IDs de grupo para especificar quem receberá uma cópia dessa mensagem de notificação.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceActionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "String (identifier)",
  "gracePeriodHours": 1024,
  "actionType": "String",
  "notificationTemplateId": "String",
  "notificationMessageCCList": [
    "String"
  ]
}
```



