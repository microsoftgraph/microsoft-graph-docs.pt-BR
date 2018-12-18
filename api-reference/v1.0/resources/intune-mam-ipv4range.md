---
title: Tipo de recurso iPv4Range
description: Intervalo de IP V4
author: tfitzmac
ms.openlocfilehash: 3dd5479776cf5f497ab6f26e893a78c73fa6ad86
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316664"
---
# <a name="ipv4range-resource-type"></a>Tipo de recurso iPv4Range

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Intervalo de IP V4

Herda de [ipRange](../resources/intune-mam-iprange.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lowerAddress|Cadeia de caracteres|Endereço IP de número mais baixo|
|upperAddress|Cadeia de caracteres|Endereço IP de número mais alto|

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



