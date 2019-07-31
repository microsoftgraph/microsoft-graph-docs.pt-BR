---
title: Tipo de recurso edgeSearchEngine
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 750208cd58a70912a437fc17ee4e2b7cc218543e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001408"
---
# <a name="edgesearchengine-resource-type"></a>Tipo de recurso edgeSearchEngine

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.


Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|edgeSearchEngineType|[edgeSearchEngineType](../resources/intune-deviceconfig-edgesearchenginetype.md)|Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM. Os valores possíveis são: `default`, `bing`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```





