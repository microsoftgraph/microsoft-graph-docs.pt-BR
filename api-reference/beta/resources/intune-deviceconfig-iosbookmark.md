---
title: tipo de recurso iosBookmark
description: indicador de URL iOS
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9d2f96b872d09eaf3c954f18a31219d6bfe17ddb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988360"
---
# <a name="iosbookmark-resource-type"></a>tipo de recurso iosBookmark

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

indicador de URL iOS

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|url|Cadeia de caracteres|URL com permissão para acessar|
|bookmarkFolder|String|A pasta na qual o indicador deve ser adicionado no Safari|
|displayName|String|O nome de exibição do indicador|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosBookmark"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosBookmark",
  "url": "String",
  "bookmarkFolder": "String",
  "displayName": "String"
}
```





