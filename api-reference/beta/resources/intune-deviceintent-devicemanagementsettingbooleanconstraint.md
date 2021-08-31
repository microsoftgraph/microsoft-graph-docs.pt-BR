---
title: Tipo de recurso deviceManagementSettingBooleanConstraint
description: Restrição da imposição de um valor booleano específico
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 63736dc3b043171b3eea3d6331386448b1f43d8d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58807269"
---
# <a name="devicemanagementsettingbooleanconstraint-resource-type"></a>Tipo de recurso deviceManagementSettingBooleanConstraint

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Restrição da imposição de um valor booleano específico


Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|valor|Boolean|O valor booleano a ser comparado com|

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



