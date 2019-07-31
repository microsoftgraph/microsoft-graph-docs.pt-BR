---
title: Tipo de recurso iPv4Range
description: Definição de intervalo IPv4.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a65489c02840960a48bb3795cada7be54abcbcca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010431"
---
# <a name="ipv4range-resource-type"></a>Tipo de recurso iPv4Range

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definição de intervalo IPv4.


Herda de [ipRange](../resources/intune-shared-iprange.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lowerAddress|String|Endereço inferior.|
|upperAddress|Cadeia de caracteres|Endereço superior.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```





