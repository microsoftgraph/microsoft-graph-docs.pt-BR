---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c618673c59ca2a085663b8b33b5585045fbc001d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273176"
---
# <a name="omasettingbase64-resource-type"></a>Tipo de recurso omaSettingBase64

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definição de Base64 das configurações de OMA.


Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome de exibição. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|description|String|Descrição. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|omaUri|Cadeia de caracteres|OMA. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|isEncrypted|Boolean|Indica se o campo de valor é criptografado. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|fileName|Cadeia de caracteres|Nome de arquivo associado com a propriedade do valor (*.cer | *. CRT | *. p7b | *. bin).|
|value|Cadeia de caracteres|Valor. (Cadeia de caracteres codificada em Base64)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "isEncrypted": true,
  "fileName": "String",
  "value": "String"
}
```




