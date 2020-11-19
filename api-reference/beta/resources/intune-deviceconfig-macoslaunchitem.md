---
title: tipo de recurso macOSLaunchItem
description: Representa um aplicativo na lista de itens de lançamento do macOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f8834b43e6d4f09e95701b700c3fa11224347291
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294302"
---
# <a name="macoslaunchitem-resource-type"></a>tipo de recurso macOSLaunchItem

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um aplicativo na lista de itens de lançamento do macOS

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|caminho|String|Caminho para o item de lançamento.|
|ocult|Booliano|Se o item será ou não ocultado da lista usuários e grupos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLaunchItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLaunchItem",
  "path": "String",
  "hide": true
}
```




