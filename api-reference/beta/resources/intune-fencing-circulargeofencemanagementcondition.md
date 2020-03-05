---
title: tipo de recurso circularGeofenceManagementCondition
description: Contém as informações para definir uma condição de gerenciamento de isolamento geográfico circular, uma área de interesse, para monitorar.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 18c1feae929fcb943b91dfd7663ee7e034d3f7d8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528189"
---
# <a name="circulargeofencemanagementcondition-resource-type"></a>tipo de recurso circularGeofenceManagementCondition

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém as informações para definir uma condição de gerenciamento de isolamento geográfico circular, uma área de interesse, para monitorar.


Herda de [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar circularGeofenceManagementConditions](../api/intune-fencing-circulargeofencemanagementcondition-list.md)|coleção [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Listar Propriedades e relações dos objetos [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .|
|[Obter circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-get.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Leia as propriedades e as relações do objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .|
|[Criar circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-create.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Criar um novo objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .|
|[Excluir circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-delete.md)|Nenhum|Exclui [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).|
|[Atualizar circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-update.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Atualiza as propriedades de um objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da condição de gerenciamento. Valor gerado pelo sistema atribuído quando criado. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|uniqueName|String|Nome exclusivo para a condição de gerenciamento. Usado em expressões de condição de gerenciamento. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|Cadeia de caracteres|O nome do administrador definido da condição de gerenciamento. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|Cadeia de caracteres|A descrição definida pelo administrador da condição de gerenciamento. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|A hora em que a condição de gerenciamento foi criada. Lado do serviço gerado. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|A hora em que a condição de gerenciamento foi modificada pela última vez. Atualizado o lado do serviço. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|ETag da condição de gerenciamento. Atualizado o lado do serviço. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|As plataformas aplicáveis para essa condição de gerenciamento. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|
|latitude|Duplo|Latitude em graus, entre-90 e + 90 inclusive.|
|longitude|Double|Longitude em graus, entre-180 e + 180 inclusive.|
|radiusInMeters|Único|RADIUS em metros.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managementConditionStatements|coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|As instruções de condição de gerenciamento associadas à condição de gerenciamento. Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.circularGeofenceManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ],
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "radiusInMeters": "<Unknown Primitive Type Edm.Single>"
}
```



