---
title: tipo de recurso keyBooleanValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor Boolean.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3ae864f951f22f74af9fb343bd78a8cd7693eb3f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705656"
---
# <a name="keybooleanvaluepair-resource-type"></a>tipo de recurso keyBooleanValuePair

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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





