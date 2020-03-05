---
title: tipo de recurso taxAreas
description: Uma área de impostos.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d2c4f007c23ae32fb79255a0a8f1509589740a70
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503429"
---
# <a name="taxareas-resource-type"></a>tipo de recurso taxAreas

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um tipo de recurso de área de imposto no Dynamics 365 Business central.

## <a name="methods"></a>Métodos
| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter taxAreas](../api/dynamics-taxarea-get.md)|taxAreas|Obtém um objeto de área de impostos.|
|[Postar taxAreas](../api/dynamics-create-taxarea.md)|taxAreas|Cria um objeto de área de impostos.|
|[Patch taxAreas](../api/dynamics-taxarea-update.md)|taxAreas|Atualiza um objeto de área de impostos.|
|[Excluir taxAreas](../api/dynamics-taxarea-delete.md)|nenhuma|Exclui um objeto de área de impostos.|

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


