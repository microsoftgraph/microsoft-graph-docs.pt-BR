---
title: tipo de recurso deviceAppManagementTask
description: Uma tarefa de gerenciamento de aplicativo de dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4097125b35f0dc5149315157d3e332204e2b1f78
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308215"
---
# <a name="deviceappmanagementtask-resource-type"></a>tipo de recurso deviceAppManagementTask

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma tarefa de gerenciamento de aplicativo de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceAppManagementTasks](../api/intune-partnerintegration-deviceappmanagementtask-list.md)|coleção [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Listar Propriedades e relações dos objetos [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) .|
|[Obter deviceAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-get.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Leia as propriedades e as relações do objeto [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) .|
|[Criar deviceAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-create.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Criar um novo objeto [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) .|
|[Excluir deviceAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-delete.md)|Nenhum|Exclui [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).|
|[Atualizar deviceAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-update.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Atualiza as propriedades de um objeto [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) .|
|[ação updateStatus](../api/intune-partnerintegration-deviceappmanagementtask-updatestatus.md)|Nenhum|Definir o status da tarefa e anexar uma anotação.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A chave da entidade.|
|displayName|String|O nome.|
|descrição|Cadeia de caracteres|A descrição.|
|createdDateTime|DateTimeOffset|A data de criação.|
|dueDateTime|DateTimeOffset|A data de conclusão.|
|category|[deviceAppManagementTaskCategory](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|A categoria. Os valores possíveis são: `unknown` e `advancedThreatProtection`.|
|prioridade|[deviceAppManagementTaskPriority](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|A prioridade. Os valores possíveis são: `none`, `high`, `low`.|
|Criador|String|O endereço de email do criador.|
|creatorNotes|String|Observações do criador.|
|assignedTo|String|O nome ou email do administrador ao qual esta tarefa é atribuída.|
|status|[deviceAppManagementTaskStatus](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|O status. Os valores possíveis são: `unknown`, `pending`, `active`, `completed`, `rejected`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagementTask"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "category": "String",
  "priority": "String",
  "creator": "String",
  "creatorNotes": "String",
  "assignedTo": "String",
  "status": "String"
}
```



