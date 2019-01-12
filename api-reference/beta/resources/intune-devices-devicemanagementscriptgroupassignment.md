---
title: tipo de recurso de deviceManagementScriptGroupAssignment
description: Contém propriedades usadas para atribuir um script de gerenciamento de dispositivo a um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8c1077cb3892cad210033abcd21a7abf2ee2e397
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934755"
---
# <a name="devicemanagementscriptgroupassignment-resource-type"></a>tipo de recurso de deviceManagementScriptGroupAssignment

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades usadas para atribuir um script de gerenciamento de dispositivo a um grupo.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista deviceManagementScriptGroupAssignments](../api/intune-devices-devicemanagementscriptgroupassignment-list.md)|coleção [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Lista as propriedades e os relacionamentos dos objetos [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .|
|[Obter deviceManagementScriptGroupAssignment](../api/intune-devices-devicemanagementscriptgroupassignment-get.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Leia as propriedades e os relacionamentos do objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .|
|[Criar deviceManagementScriptGroupAssignment](../api/intune-devices-devicemanagementscriptgroupassignment-create.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Crie um novo objeto de [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .|
|[Excluir deviceManagementScriptGroupAssignment](../api/intune-devices-devicemanagementscriptgroupassignment-delete.md)|Nenhum|Exclui um [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).|
|[Atualizar deviceManagementScriptGroupAssignment](../api/intune-devices-devicemanagementscriptgroupassignment-update.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Atualize as propriedades de um objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade de atribuição de grupo de script para gerenciamento do dispositivo.|
|targetGroupId|String|A Id de grupo do Active Directory do Windows Azure Pretendemos o script.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```





