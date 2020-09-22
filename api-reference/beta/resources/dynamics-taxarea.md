---
title: tipo de recurso taxAreas
description: Uma área de impostos.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 140470f0e293b41770779628280f0117d8bb6a89
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027052"
---
# <a name="taxareas-resource-type"></a>tipo de recurso taxAreas

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um tipo de recurso de área de imposto no Dynamics 365 Business central.

## <a name="methods"></a>Métodos
| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter taxAreas](../api/dynamics-taxarea-get.md)|taxAreas|Obtém um objeto de área de impostos.|
|[Postar taxAreas](../api/dynamics-create-taxarea.md)|taxAreas|Cria um objeto de área de impostos.|
|[Patch taxAreas](../api/dynamics-taxarea-update.md)|taxAreas|Atualiza um objeto de área de impostos.|
|[Excluir taxAreas](../api/dynamics-taxarea-delete.md)|Nenhuma|Exclui um objeto de área de impostos.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|GUID|A identificação exclusiva da área de impostos. Não editável.|
|código|Cadeia de caracteres, tamanho máximo 20| O código da área de impostos.|
|displayName|Cadeia de caracteres, tamanho máximo 50| O nome de exibição da área de impostos.|
|taxType|string|O tipo de imposto da área de impostos.|
|lastModifiedDateTime|datetime|A última data/hora em que a área de impostos foi modificada. Somente leitura.|

## <a name="relationships"></a>Relações

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "taxType": "String",
  "lastModifiedDateTime": "datetime"
}
```




