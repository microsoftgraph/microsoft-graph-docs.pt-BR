---
title: tipo de recurso de managementCondition
description: Condições de gerenciamento são eventos que podem ser disparados dinamicamente como limites de geo, limites de tempo e limites de rede.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c41b4cb3143349ba0fdd97633a70ec7b38e266ec
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405853"
---
# <a name="managementcondition-resource-type"></a>tipo de recurso de managementCondition

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Condições de gerenciamento são eventos que podem ser disparados dinamicamente como limites de geo, limites de tempo e limites de rede.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista managementConditions](../api/intune-fencing-managementcondition-list.md)|coleção [managementCondition](../resources/intune-fencing-managementcondition.md)|Lista as propriedades e os relacionamentos dos objetos [managementCondition](../resources/intune-fencing-managementcondition.md) .|
|[Obter managementCondition](../api/intune-fencing-managementcondition-get.md)|[managementCondition](../resources/intune-fencing-managementcondition.md)|Leia as propriedades e os relacionamentos do objeto [managementCondition](../resources/intune-fencing-managementcondition.md) .|
|[função getManagementConditionsForPlatform](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|coleção [managementCondition](../resources/intune-fencing-managementcondition.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para a condição de gerenciamento. Valor atribuído quando criado gerado pelo sistema.|
|nome exclusivo|String|Nome exclusivo para a condição de gerenciamento. Usadas nas expressões de condição de gerenciamento.|
|displayName|String|O nome definido admin da condição de gerenciamento.|
|description|String|O administrador definidos descrição da condição de gerenciamento.|
|createdDateTime|DateTimeOffset|A hora em que a condição de gerenciamento foi criada. Lado de serviço gerado.|
|modifiedDateTime|DateTimeOffset|A hora que da última modificação a condição de gerenciamento. Lado de serviços atualizado.|
|eTag|String|ETag da condição de gerenciamento. Lado de serviços atualizado.|
|applicablePlatforms|coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|As plataformas aplicáveis para essa condição de gerenciamento.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managementConditionStatements|coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|As instruções de condição de gerenciamento associadas à condição de gerenciamento.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCondition",
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




