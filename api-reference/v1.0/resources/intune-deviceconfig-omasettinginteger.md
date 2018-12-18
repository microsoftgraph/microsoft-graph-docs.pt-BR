---
title: Tipo de recurso omaSettingInteger
description: Definição de números inteiros das configurações de OMA.
author: tfitzmac
ms.openlocfilehash: 6a2e6fe6e6782159afa99d91785ae9e854a2e99c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306549"
---
# <a name="omasettinginteger-resource-type"></a>Tipo de recurso omaSettingInteger

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Definição de números inteiros das configurações de OMA.

Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome de exibição. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|descrição|Cadeia de caracteres|Descrição. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|omaUri|Cadeia de caracteres|OMA. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|valor|Int32|Valor.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```



