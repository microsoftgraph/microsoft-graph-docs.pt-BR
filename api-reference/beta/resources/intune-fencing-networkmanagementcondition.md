---
title: Tipo de recurso networkManagementCondition
description: Contém as informações para definir uma condição de gerenciamento de rede.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8e7c23fb6806ba5065f28757fcab57f45b8492b6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58791106"
---
# <a name="networkmanagementcondition-resource-type"></a>Tipo de recurso networkManagementCondition

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém as informações para definir uma condição de gerenciamento de rede.


Herda de [managementCondition](../resources/intune-fencing-managementcondition.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar networkManagementConditions](../api/intune-fencing-networkmanagementcondition-list.md)|[coleção networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)|Listar propriedades e relações dos objetos [networkManagementCondition.](../resources/intune-fencing-networkmanagementcondition.md)|
|[Obter networkManagementCondition](../api/intune-fencing-networkmanagementcondition-get.md)|[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)|Leia propriedades e relações do [objeto networkManagementCondition.](../resources/intune-fencing-networkmanagementcondition.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da condição de gerenciamento. Valor gerado pelo sistema atribuído quando criado. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|Nome único|Cadeia de caracteres|Nome exclusivo para a condição de gerenciamento. Usado em expressões de condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|Cadeia de caracteres|O nome definido pelo administrador da condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|descrição|Cadeia de caracteres|A descrição definida pelo administrador da condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
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
  "@odata.type": "microsoft.graph.networkManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkManagementCondition",
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



