---
title: Tipo de recurso cloudPcSupportedRegion
description: Representa uma região com suporte para estabelecer uma conexão de rede do Azure para PCs de Nuvem.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: d13bfb6709d856119dcfaa700d819b9ed6f55258
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588565"
---
# <a name="cloudpcsupportedregion-resource-type"></a>Tipo de recurso cloudPcSupportedRegion

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma região com suporte para estabelecer uma conexão de rede do Azure para PCs de Nuvem.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar cloudPcSupportedRegions](../api/virtualendpoint-list-supportedregions.md)|[coleção cloudPcSupportedRegion](../resources/cloudpcsupportedregion.md)|Listar as regiões com suporte disponíveis para a criação de conexões de computador na nuvem.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da região com suporte. Somente leitura.|
|displayName|Cadeia de caracteres|O nome da região com suporte. Somente leitura.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcSupportedRegion",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSupportedRegion",
  "id": "String (identifier)",
  "displayName": "String"
}
```
