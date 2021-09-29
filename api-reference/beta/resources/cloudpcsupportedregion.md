---
title: Tipo de recurso cloudPcSupportedRegion
description: Representa uma região com suporte para estabelecer uma conexão de rede local para PCs na Nuvem.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 150138b8be51fd8b333cb100aaa65dbbcd8bdfc6
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59997223"
---
# <a name="cloudpcsupportedregion-resource-type"></a>Tipo de recurso cloudPcSupportedRegion

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma região com suporte para estabelecer uma conexão de rede local para PCs na Nuvem.

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
