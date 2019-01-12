---
title: Tipo de recurso iPv6Range
description: Intervalo de IPV6
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2c30d85a83bb604a5c0ccb6563d6315a183f6497
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971477"
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



