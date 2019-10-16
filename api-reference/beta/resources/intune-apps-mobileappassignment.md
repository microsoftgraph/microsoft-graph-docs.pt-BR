---
title: Tipo de recurso mobileAppAssignment
description: Uma classe com as propriedades usadas para atribuição de grupos de um aplicativo móvel.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e2284ac4cd722193487e19af11abbb90d6f01af3
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538564"
---
# <a name="mobileappassignment-resource-type"></a>Tipo de recurso mobileAppAssignment

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe com as propriedades usadas para atribuição de grupos de um aplicativo móvel.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppAssignments](../api/intune-apps-mobileappassignment-list.md)|Conjunto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Listar propriedades e relações de objetos de [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|
|[Obter mobileAppAssignment](../api/intune-apps-mobileappassignment-get.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Ler propriedades e relações de objetos de [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|
|[Criar mobileAppAssignment](../api/intune-apps-mobileappassignment-create.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Criar um novo objeto de [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|
|[Excluir mobileAppAssignment](../api/intune-apps-mobileappassignment-delete.md)|Nenhum|Excluir uma [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|
|[Atualizar mobileAppAssignment](../api/intune-apps-mobileappassignment-update.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Atualizar as propriedades de um objeto de [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|finalidade|[installIntent](../resources/intune-shared-installintent.md)|A finalidade da instalação definida pelo administrador. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|A atribuição do grupo de destino definida pelo administrador.|
|configurações|[mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)|As configurações para a atribuição de destino definida pelo administrador.|
|source|[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|O tipo de recurso que é a origem da atribuição. Os valores possíveis são: `direct` e `policySets`.|
|sourceId|Cadeia de caracteres|O identificador da origem da atribuição.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "String (identifier)",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  },
  "source": "String",
  "sourceId": "String"
}
```



