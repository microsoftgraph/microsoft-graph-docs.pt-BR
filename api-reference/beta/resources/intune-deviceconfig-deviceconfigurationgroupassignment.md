---
title: Tipo de recurso deviceConfigurationGroupAssignment
description: Atribuição de grupo de configuração de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bd2bc078ed2b3d6fc55b77d82c01422a8febf34df25632cbb91dd1c66f070522
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54122666"
---
# <a name="deviceconfigurationgroupassignment-resource-type"></a>Tipo de recurso deviceConfigurationGroupAssignment

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atribuição de grupo de configuração de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceConfigurationGroupAssignments](../api/intune-deviceconfig-deviceconfigurationgroupassignment-list.md)|[Coleção deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Listar propriedades e relações dos [objetos deviceConfigurationGroupAssignment.](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|
|[Obter deviceConfigurationGroupAssignment](../api/intune-deviceconfig-deviceconfigurationgroupassignment-get.md)|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Leia propriedades e relações do [objeto deviceConfigurationGroupAssignment.](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|
|[Criar deviceConfigurationGroupAssignment](../api/intune-deviceconfig-deviceconfigurationgroupassignment-create.md)|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Crie um novo [objeto deviceConfigurationGroupAssignment.](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|
|[Excluir deviceConfigurationGroupAssignment](../api/intune-deviceconfig-deviceconfigurationgroupassignment-delete.md)|Nenhum|Exclui um [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).|
|[Atualizar deviceConfigurationGroupAssignment](../api/intune-deviceconfig-deviceconfigurationgroupassignment-update.md)|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Atualize as propriedades de [um objeto deviceConfigurationGroupAssignment.](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|targetGroupId|Cadeia de caracteres|A ID do grupo AAD para o que estamos direcionando a configuração do dispositivo.|
|excludeGroup|Boolean|Indica se esse grupo deve ser excluído. Padrões de que o grupo deve ser incluído|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deviceConfiguration|[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|O link de navegação para a Configuração do Dispositivo que está sendo direcionada.|

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




