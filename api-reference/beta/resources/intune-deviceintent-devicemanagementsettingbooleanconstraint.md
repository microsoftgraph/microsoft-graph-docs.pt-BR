---
title: tipo de recurso deviceManagementSettingBooleanConstraint
description: Restrição o impõe um valor booliano específico
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9a83a0747e0960aeebaa0de472fae4d587111946
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364723"
---
# <a name="devicemanagementsettingbooleanconstraint-resource-type"></a>tipo de recurso deviceManagementSettingBooleanConstraint

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Restrição o impõe um valor booliano específico


Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|valor|Boolean|O valor booliano a ser comparado|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingBooleanConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingBooleanConstraint",
  "value": true
}
```



