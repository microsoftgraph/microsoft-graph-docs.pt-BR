---
title: tipo de recurso deviceManagementEnumValue
description: Informações de definição para um valor de enumeração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 86a97937872bd46e2fd71c781e90ba607f5baf9d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49275913"
---
# <a name="devicemanagementenumvalue-resource-type"></a>tipo de recurso deviceManagementEnumValue

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Informações de definição para um valor de enumeração

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|valor|Cadeia de caracteres|O texto de valor de enumeração bruto|
|displayName|String|Nome para exibição desse valor de enumeração|

## <a name="relationships"></a>Relações
Nenhum

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




