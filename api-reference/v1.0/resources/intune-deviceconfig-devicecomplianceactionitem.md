---
title: Tipo de recurso deviceComplianceActionItem
description: Configuração de ação agendada
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1b0a507ffb080f2354e5c854810554da64b47e7c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254685"
---
# <a name="devicecomplianceactionitem-resource-type"></a>Tipo de recurso deviceComplianceActionItem

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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
|actionType|[Enumeraçãodevicecomplianceactiontype](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|Qual ação executar. Os valores possíveis são: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.|
|notificationTemplateId|Cadeia de caracteres|Qual modelo de notificação de mensagem será usado|
|notificationMessageCCList|Coleção de cadeias de caracteres|Uma lista de IDs de grupo para especificar quem receberá uma cópia dessa mensagem de notificação.|

## <a name="relationships"></a>Relações
Nenhuma

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



