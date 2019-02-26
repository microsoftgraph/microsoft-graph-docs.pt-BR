---
title: Tipo de recurso omaSettingDateTime
description: Definição de datetime para configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20bc82e88480dca1df727e299e62c4274002176f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260911"
---
# <a name="omasettingdatetime-resource-type"></a>Tipo de recurso omaSettingDateTime

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definição de datetime para configurações de OMA.


Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome de exibição. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|descrição|String|Descrição. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|omaUri|Cadeia de caracteres|OMA. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|value|DateTimeOffset|Valor.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```



