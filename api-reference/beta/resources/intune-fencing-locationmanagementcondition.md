---
title: tipo de recurso locationManagementCondition
description: Contém as informações para definir uma condição de gerenciamento de local, uma área de interesse, a ser monitorada.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b6a2e4bad74257f91b487ee720665c29b7518294
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030281"
---
# <a name="locationmanagementcondition-resource-type"></a>tipo de recurso locationManagementCondition

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém as informações para definir uma condição de gerenciamento de local, uma área de interesse, a ser monitorada.


Herda de [managementCondition](../resources/intune-fencing-managementcondition.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar locationManagementConditions](../api/intune-fencing-locationmanagementcondition-list.md)|[coleção locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)|Listar propriedades e relações dos [objetos locationManagementCondition.](../resources/intune-fencing-locationmanagementcondition.md)|
|[Obter locationManagementCondition](../api/intune-fencing-locationmanagementcondition-get.md)|[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)|Leia propriedades e relações do [objeto locationManagementCondition.](../resources/intune-fencing-locationmanagementcondition.md)|

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

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managementConditionStatements|[coleção managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|As instruções de condição de gerenciamento associadas à condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.locationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locationManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```



