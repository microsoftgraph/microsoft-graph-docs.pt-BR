---
title: tipo de recurso deviceManagementEnumValue
description: Informações de definição para um valor de enumeração
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de1340223d45361825b2b8d8fc4e57194437f6b6
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523732"
---
# <a name="devicemanagementenumvalue-resource-type"></a>tipo de recurso deviceManagementEnumValue

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Informações de definição para um valor de enumeração

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|value|Cadeia de caracteres|O texto de valor de enumeração bruto|
|displayName|String|Nome para exibição desse valor de enumeração|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementEnumValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementEnumValue",
  "value": "String",
  "displayName": "String"
}
```







