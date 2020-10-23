---
title: tipo de recurso deviceManagementScriptGroupAssignment
description: Contém propriedades usadas para atribuir um script de gerenciamento de dispositivo a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b6d7e0b274f289b85e6add646f9444c4697f8a25
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691397"
---
# <a name="devicemanagementscriptgroupassignment-resource-type"></a>tipo de recurso deviceManagementScriptGroupAssignment

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades usadas para atribuir um script de gerenciamento de dispositivo a um grupo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementScriptGroupAssignments](../api/intune-devices-devicemanagementscriptgroupassignment-list.md)|coleção [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Listar Propriedades e relações dos objetos [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .|
|[Obter deviceManagementScriptGroupAssignment](../api/intune-devices-devicemanagementscriptgroupassignment-get.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Leia as propriedades e as relações do objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .|
|[Criar deviceManagementScriptGroupAssignment](../api/intune-devices-devicemanagementscriptgroupassignment-create.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Criar um novo objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .|
|[Excluir deviceManagementScriptGroupAssignment](../api/intune-devices-devicemanagementscriptgroupassignment-delete.md)|Nenhum|Exclui [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).|
|[Atualizar deviceManagementScriptGroupAssignment](../api/intune-devices-devicemanagementscriptgroupassignment-update.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Atualiza as propriedades de um objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade de atribuição do grupo de scripts de gerenciamento de dispositivos. Essa propriedade é somente leitura.|
|targetGroupId|String|A ID do grupo do Azure Active Directory para o qual estamos direcionando o script.|

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





