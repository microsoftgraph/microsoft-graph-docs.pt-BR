---
title: tipo de recurso officeClientConfigurationAssignment
description: Atribuição de configuração de cliente do Office.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 96b7ef0ad1374b6da2671c191b427a988b8b2f2a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708953"
---
# <a name="officeclientconfigurationassignment-resource-type"></a>tipo de recurso officeClientConfigurationAssignment

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atribuição de configuração de cliente do Office.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar officeClientConfigurationAssignments](../api/intune-cirrus-officeclientconfigurationassignment-list.md)|coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Listar Propriedades e relações dos objetos [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .|
|[Obter officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-get.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Leia as propriedades e as relações do objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .|
|[Criar officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-create.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Criar um novo objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .|
|[Excluir officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-delete.md)|Nenhum|Exclui [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).|
|[Atualizar officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-update.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Atualiza as propriedades de um objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID do OfficeConfigurationAssignment.|
|destino|[officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|A atribuição de destino definida pelo administrador.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```





