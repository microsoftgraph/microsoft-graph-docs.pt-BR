---
title: Tipo de recurso keyStringValuePair
description: Um par de valores-chave com uma chave de cadeia de caracteres e um valor de cadeia de caracteres.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cfd28c44c98504e3fc83b5cfcebd5a8ec0e459c1
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58801119"
---
# <a name="keystringvaluepair-resource-type"></a>Tipo de recurso keyStringValuePair

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um par de valores-chave com uma chave de cadeia de caracteres e um valor de cadeia de caracteres.


Herda de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|key|Cadeia de caracteres|A chave de cadeia de caracteres do par de valores-chave. Herdado de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)|
|value|Cadeia de caracteres|O valor da cadeia de caracteres do par de valores-chave.|

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



