---
title: tipo de recurso macOSSystemExtension
description: Representa uma extensão de sistema macOS específica.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bab537a60d213e2e1976c8f902ce7a8b0dbc3027
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179401"
---
# <a name="macossystemextension-resource-type"></a>tipo de recurso macOSSystemExtension

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa uma extensão de sistema macOS específica.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|teamIdentifier|Cadeia de Caracteres|Obtém ou define o identificador de equipe que foi usado para assinar a extensão do sistema.|
|bundleId|String|Obtém ou define o identificador de pacote da extensão do sistema.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSSystemExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSystemExtension",
  "teamIdentifier": "String",
  "bundleId": "String"
}
```



