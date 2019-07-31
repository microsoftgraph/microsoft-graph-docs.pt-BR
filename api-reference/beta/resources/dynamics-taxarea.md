---
title: tipo de recurso taxAreas
description: Uma área de impostos.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 09c1c51fed961489d824136f28aaa2f5b3859b44
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972891"
---
# <a name="taxareas-resource-type"></a>tipo de recurso taxAreas
Representa um tipo de recurso de área de imposto no Dynamics 365 Business central.

## <a name="methods"></a>Métodos
| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter taxAreas](../api/dynamics-taxarea-get.md)|taxAreas|Obtém um objeto de área de impostos.|
|[Postar taxAreas](../api/dynamics-create-taxarea.md)|taxAreas|Cria um objeto de área de impostos.|
|[Patch taxAreas](../api/dynamics-taxarea-update.md)|taxAreas|Atualiza um objeto de área de impostos.|
|[Excluir taxAreas](../api/dynamics-taxarea-delete.md)|none|Exclui um objeto de área de impostos.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|GUID|A identificação exclusiva da área de impostos. Não editável.|
|código|Cadeia de caracteres, tamanho máximo 20| O código da área de impostos.|
|displayName|Cadeia de caracteres, tamanho máximo 50| O nome de exibição da área de impostos.|
|taxType|string|O tipo de imposto da área de impostos.|
|lastModifiedDateTime|DateTime|A última data/hora em que a área de impostos foi modificada. Somente leitura.|

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


