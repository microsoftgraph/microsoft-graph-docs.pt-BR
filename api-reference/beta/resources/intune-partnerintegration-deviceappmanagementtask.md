---
title: Tipo de recurso deviceAppManagementTask
description: Uma tarefa de gerenciamento de aplicativo de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c539c1c2ee284641e7f63f0113ebc35f5ea866f3087339cf436f5f783c830be2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54164164"
---
# <a name="deviceappmanagementtask-resource-type"></a>Tipo de recurso deviceAppManagementTask

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma tarefa de gerenciamento de aplicativo de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceAppManagementTasks](../api/intune-partnerintegration-deviceappmanagementtask-list.md)|[Coleção deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Listar propriedades e relações dos [objetos deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|[Obter deviceAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-get.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Leia propriedades e relações do [objeto deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|[Criar deviceAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-create.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Crie um novo [objeto deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|[Excluir deviceAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-delete.md)|Nenhum|Exclui um [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).|
|[Atualizar deviceAppManagementTask](../api/intune-partnerintegration-deviceappmanagementtask-update.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Atualize as propriedades de [um objeto deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|[Ação updateStatus](../api/intune-partnerintegration-deviceappmanagementtask-updatestatus.md)|Nenhum|De definir o status da tarefa e anexar uma nota.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A chave da entidade.|
|displayName|Cadeia de caracteres|O nome.|
|description|Cadeia de caracteres|A descrição.|
|createdDateTime|DateTimeOffset|A data criada.|
|dueDateTime|DateTimeOffset|A data de vencimento.|
|category|[deviceAppManagementTaskCategory](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|A categoria. Os valores possíveis são: `unknown` e `advancedThreatProtection`.|
|prioridade|[deviceAppManagementTaskPriority](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|A prioridade. Os valores possíveis são: `none`, `high`, `low`.|
|criador|Cadeia de caracteres|O endereço de email do criador.|
|creatorNotes|Cadeia de caracteres|Observações do criador.|
|assignedTo|Cadeia de caracteres|O nome ou o email do administrador ao que essa tarefa é atribuída.|
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




