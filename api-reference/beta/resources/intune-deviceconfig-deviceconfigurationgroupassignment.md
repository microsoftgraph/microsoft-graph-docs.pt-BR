---
title: tipo de recurso deviceConfigurationGroupAssignment
description: Atribuição de grupo de configuração de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eafc10e4fb464ab9dbaee642816b56a761bb5516
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469378"
---
# <a name="deviceconfigurationgroupassignment-resource-type"></a>tipo de recurso deviceConfigurationGroupAssignment

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atribuição de grupo de configuração de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceConfigurationGroupAssignments](../api/intune-deviceconfig-deviceconfigurationgroupassignment-list.md)|coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Listar Propriedades e relações dos objetos [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .|
|[Obter deviceConfigurationGroupAssignment](../api/intune-deviceconfig-deviceconfigurationgroupassignment-get.md)|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Leia as propriedades e as relações do objeto [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .|
|[Criar deviceConfigurationGroupAssignment](../api/intune-deviceconfig-deviceconfigurationgroupassignment-create.md)|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Criar um novo objeto [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .|
|[Excluir deviceConfigurationGroupAssignment](../api/intune-deviceconfig-deviceconfigurationgroupassignment-delete.md)|Nenhum|Exclui [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).|
|[Atualizar deviceConfigurationGroupAssignment](../api/intune-deviceconfig-deviceconfigurationgroupassignment-update.md)|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Atualiza as propriedades de um objeto [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|targetGroupId|String|A ID do grupo do AAD no qual estamos direcionando a configuração do dispositivo.|
|excludeGroup|Booliano|Indica se esse grupo deve ser excluído. Padrões que o grupo deve ser incluído|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deviceConfiguration|[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|O link de navegação para a configuração do dispositivo que está sendo direcionada.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String",
  "excludeGroup": true
}
```



