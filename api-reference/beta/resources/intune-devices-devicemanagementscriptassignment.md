---
title: tipo de recurso deviceManagementScriptAssignment
description: Contém propriedades usadas para atribuir um script de gerenciamento de dispositivo a um grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 22286eac6abc1ebad7ecc839eed9c872c70ff602
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196984"
---
# <a name="devicemanagementscriptassignment-resource-type"></a>tipo de recurso deviceManagementScriptAssignment

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades usadas para atribuir um script de gerenciamento de dispositivo a um grupo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementScriptAssignments](../api/intune-devices-devicemanagementscriptassignment-list.md)|coleção [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|Listar Propriedades e relações dos objetos [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .|
|[Obter deviceManagementScriptAssignment](../api/intune-devices-devicemanagementscriptassignment-get.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|Leia as propriedades e as relações do objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .|
|[Criar deviceManagementScriptAssignment](../api/intune-devices-devicemanagementscriptassignment-create.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|Criar um novo objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .|
|[Excluir deviceManagementScriptAssignment](../api/intune-devices-devicemanagementscriptassignment-delete.md)|Nenhum|Exclui [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).|
|[Atualizar deviceManagementScriptAssignment](../api/intune-devices-devicemanagementscriptassignment-update.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|Atualiza as propriedades de um objeto [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade de atribuição do grupo de scripts de gerenciamento de dispositivos. Essa propriedade é somente leitura.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|A ID do grupo do Azure Active Directory para o qual estamos direcionando o script.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



