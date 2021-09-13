---
title: tipo de recurso circularGeofenceManagementCondition
description: Contém as informações para definir uma condição de gerenciamento de cerca geográfica circular, uma área de interesse, a ser monitorada.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 32032ef83f3a724ecc98fd1134d40d95b1a76dcf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030295"
---
# <a name="circulargeofencemanagementcondition-resource-type"></a>tipo de recurso circularGeofenceManagementCondition

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém as informações para definir uma condição de gerenciamento de cerca geográfica circular, uma área de interesse, a ser monitorada.


Herda [de locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar circularGeofenceManagementConditions](../api/intune-fencing-circulargeofencemanagementcondition-list.md)|[coleção circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Listar propriedades e relações dos [objetos circularGeofenceManagementCondition.](../resources/intune-fencing-circulargeofencemanagementcondition.md)|
|[Obter circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-get.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Leia propriedades e relações do [objeto circularGeofenceManagementCondition.](../resources/intune-fencing-circulargeofencemanagementcondition.md)|
|[Criar circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-create.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Crie um novo [objeto circularGeofenceManagementCondition.](../resources/intune-fencing-circulargeofencemanagementcondition.md)|
|[Excluir circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-delete.md)|Nenhum|Exclui [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).|
|[Atualizar circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-update.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Atualize as propriedades de [um objeto circularGeofenceManagementCondition.](../resources/intune-fencing-circulargeofencemanagementcondition.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da condição de gerenciamento. Valor gerado pelo sistema atribuído quando criado. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|Nome único|Cadeia de caracteres|Nome exclusivo para a condição de gerenciamento. Usado em expressões de condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|Cadeia de caracteres|O nome definido pelo administrador da condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|Cadeia de caracteres|A descrição definida pelo administrador da condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|A hora em que a condição de gerenciamento foi criada. Lado de serviço gerado. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|O tempo em que a condição de gerenciamento foi modificada pela última vez. Lado do serviço atualizado. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|ETag da condição de gerenciamento. Lado do serviço atualizado. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[Coleção devicePlatformType](../resources/intune-fencing-deviceplatformtype.md)|As plataformas aplicáveis para essa condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|latitude|Double|Latitude em graus, entre -90 e +90 inclusive.|
|longitude|Double|Longitude em graus, entre -180 e +180 inclusive.|
|radiusInMeters|Simples|Raio em metros.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managementConditionStatements|[coleção managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|As instruções de condição de gerenciamento associadas à condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|

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
  "latitude": "4.2",
  "longitude": "4.2",
  "radiusInMeters": 4.2
}
```



