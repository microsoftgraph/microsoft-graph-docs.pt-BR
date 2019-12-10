---
title: tipo de recurso keyStringValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor de cadeia de caracteres.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7c62ec2cf1fbe5a78534bdb5f6ff9b1e73e37c9f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39924518"
---
# <a name="keystringvaluepair-resource-type"></a>tipo de recurso keyStringValuePair

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um par chave-valor com uma chave de cadeia de caracteres e um valor de cadeia de caracteres.


Herda de [keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|key|Cadeia de Caracteres|A chave de cadeia de caracteres do par chave-valor. Herdado de [keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)|
|value|Cadeia de caracteres|O valor da cadeia de caracteres do par chave-valor.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyStringValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyStringValuePair",
  "key": "String",
  "value": "String"
}
```



