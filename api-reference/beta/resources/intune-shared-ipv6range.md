---
title: Tipo de recurso iPv6Range
description: Intervalo de IPV6
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 759f661464d2dd5cd6c12f6fbfe6b1bfcf549a70
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829656"
---
# <a name="ipv6range-resource-type"></a>Tipo de recurso iPv6Range

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Intervalo de IPV6

Herda de [ipRange](../resources/intune-shared-iprange.md)

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
  "keyProperty": "id",
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



