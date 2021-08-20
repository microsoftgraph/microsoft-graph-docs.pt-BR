---
title: Tipo de recurso deviceManagementSettingBooleanConstraint
description: Restrição da imposição de um valor booleano específico
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 32a0dcf4d65df9375aff4aab865535f98999c3015f470bf9ecb368867a4840ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54122492"
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




