---
title: tipo de recurso de managementCondition
description: Condições de gerenciamento são eventos que podem ser disparados dinamicamente como limites de geo, limites de tempo e limites de rede.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: e0aeb73a93cd4c61b6d4680f73c2a9b8cee830c6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986737"
---
# <a name="managementcondition-resource-type"></a>tipo de recurso de managementCondition

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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
|id|Cadeia de caracteres|Identificador exclusivo para a condição de gerenciamento. Valor atribuído quando criado gerado pelo sistema.|
|nome exclusivo|Cadeia de caracteres|Nome exclusivo para a condição de gerenciamento. Usadas nas expressões de condição de gerenciamento.|
|displayName|Cadeia de caracteres|O nome definido admin da condição de gerenciamento.|
|description|Cadeia de caracteres|O administrador definidos descrição da condição de gerenciamento.|
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





