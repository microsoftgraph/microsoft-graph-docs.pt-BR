---
title: tipo de recurso keyBooleanValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor Boolean.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c525c1880c8a77dd8bf29c1ee5c8fb2864ab928b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199690"
---
# <a name="keybooleanvaluepair-resource-type"></a>tipo de recurso keyBooleanValuePair

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um par chave-valor com uma chave de cadeia de caracteres e um valor Boolean.


Herda de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|key|String|A chave de cadeia de caracteres do par chave-valor. Herdado de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)|
|value|Boolean|O valor booliano do par chave-valor.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyBooleanValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyBooleanValuePair",
  "key": "String",
  "value": true
}
```



