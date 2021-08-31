---
title: Tipo de recurso keyLongValuePair
description: Par de valores longos da chave
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7d0e2f624dcaffa9706f241814e5185a1bcb6341
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58786716"
---
# <a name="keylongvaluepair-resource-type"></a>Tipo de recurso keyLongValuePair

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Par de valores longos da chave

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|nome|Cadeia de caracteres|Nome para esse par de valores longos de chave|
|valor|Int64|Valor para esse par de valores longos de chave|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyLongValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyLongValuePair",
  "name": "String",
  "value": 1024
}
```



