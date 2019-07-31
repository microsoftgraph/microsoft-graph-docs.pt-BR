---
title: Tipo de recurso iPv6Range
description: Definição de intervalo IPv6.
author: rolyon
localization_priority: Normal
doc_type: resourcePageType
ms.prod: Intune
ms.openlocfilehash: 1f2b46cea71d097955ca9e78cc74f6f0cddd1002
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967366"
---
# <a name="ipv6range-resource-type"></a>Tipo de recurso iPv6Range

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definição de intervalo IPv6.


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
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```





