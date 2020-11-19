---
title: tipo de recurso deviceManagementSettingAbstractImplementationConstraint
description: A restrição que impõe um tipo de AbstractComplex tem ou está definida para um valor específico
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 89ea13dc05537c51fc5e3e0effaab11fc874419b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49275605"
---
# <a name="devicemanagementsettingabstractimplementationconstraint-resource-type"></a>tipo de recurso deviceManagementSettingAbstractImplementationConstraint

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A restrição que impõe um tipo de AbstractComplex tem ou está definida para um valor específico


Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAbstractImplementationDefinitionIds|Coleção de cadeias de caracteres|Lista de valores que significa não configurado para a configuração|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingAbstractImplementationConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingAbstractImplementationConstraint",
  "allowedAbstractImplementationDefinitionIds": [
    "String"
  ]
}
```




