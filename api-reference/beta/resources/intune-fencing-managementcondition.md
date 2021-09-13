---
title: Tipo de recurso managementCondition
description: Condições de gerenciamento são eventos que podem ser disparados dinamicamente, como cercas geográficas, cercas de tempo e cercas de rede.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8db902ca0f5b0fb00a72e9fd8eee8af02d2c8cab
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030253"
---
# <a name="managementcondition-resource-type"></a>Tipo de recurso managementCondition

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Condições de gerenciamento são eventos que podem ser disparados dinamicamente, como cercas geográficas, cercas de tempo e cercas de rede.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Gerenciamento de listasConditions](../api/intune-fencing-managementcondition-list.md)|[coleção managementCondition](../resources/intune-fencing-managementcondition.md)|Listar propriedades e relações dos objetos [managementCondition.](../resources/intune-fencing-managementcondition.md)|
|[Obter managementCondition](../api/intune-fencing-managementcondition-get.md)|[managementCondition](../resources/intune-fencing-managementcondition.md)|Leia propriedades e relações do [objeto managementCondition.](../resources/intune-fencing-managementcondition.md)|
|[função getManagementConditionsForPlatform](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|[coleção managementCondition](../resources/intune-fencing-managementcondition.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da condição de gerenciamento. Valor gerado pelo sistema atribuído quando criado.|
|Nome único|Cadeia de caracteres|Nome exclusivo para a condição de gerenciamento. Usado em expressões de condição de gerenciamento.|
|displayName|Cadeia de caracteres|O nome definido pelo administrador da condição de gerenciamento.|
|description|Cadeia de caracteres|A descrição definida pelo administrador da condição de gerenciamento.|
|createdDateTime|DateTimeOffset|A hora em que a condição de gerenciamento foi criada. Lado de serviço gerado.|
|modifiedDateTime|DateTimeOffset|O tempo em que a condição de gerenciamento foi modificada pela última vez. Lado do serviço atualizado.|
|eTag|String|ETag da condição de gerenciamento. Lado do serviço atualizado.|
|applicablePlatforms|[Coleção devicePlatformType](../resources/intune-fencing-deviceplatformtype.md)|As plataformas aplicáveis para essa condição de gerenciamento.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managementConditionStatements|[coleção managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|As instruções de condição de gerenciamento associadas à condição de gerenciamento.|

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



