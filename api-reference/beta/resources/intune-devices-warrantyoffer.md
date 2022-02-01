---
title: Tipo de recurso warrantyOffer
description: Modelos e Manufaturas de carmadata para dispositivos gerenciados na conta
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7f8045dcc99c2c9e28099a39e54baa1e0561b5d2
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292270"
---
# <a name="warrantyoffer-resource-type"></a>Tipo de recurso warrantyOffer

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Modelos e Manufaturas de carmadata para dispositivos gerenciados na conta

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|type|[warrantyType](../resources/intune-devices-warrantytype.md)|Tipo de oferta de garantia. Os valores possíveis são: `unknown`, `manufacturer`, `contractual`, `unknownFutureValue`.|
|description|Cadeia de caracteres|Descrição da oferta de garantia|
|startDateTime|DateTimeOffset|Data de início da oferta de garantia|
|endDateTime|DateTimeOffset|Data de término da oferta de garantia|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.warrantyOffer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.warrantyOffer",
  "type": "String",
  "description": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```




