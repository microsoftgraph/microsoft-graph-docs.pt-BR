---
title: tipo de recurso keyBooleanValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor Boolean.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aabdb6e8eef4e41ec5c9aaf5d1a24fca97ae8c2e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526266"
---
# <a name="keybooleanvaluepair-resource-type"></a>tipo de recurso keyBooleanValuePair

Namespace: Microsoft. Graph

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



