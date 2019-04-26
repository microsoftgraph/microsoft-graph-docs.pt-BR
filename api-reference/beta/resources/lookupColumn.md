---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
ms.openlocfilehash: 04b9a92bfd723b188fc6869717a5665e10b6af30
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345177"
---
# <a name="lookupcolumn-resource-type"></a>Tipo de recurso LookupColumn

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A **lookupColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são buscados em outra origem do site.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **lookupColumn**.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.lookupColumn" } -->

```json
{
  "allowMultipleValues": true,
  "allowUnlimitedLength": false,
  "columnName": "string",
  "listId": "string",
  "primaryLookupColumnId": "string"
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade             | Tipo    | Descrição
|:--------------------------|:--------|:---------------------------------------
| **allowMultipleValues**   | booliano | Indica se vários valores podem ser selecionados da origem.
| **allowUnlimitedLength**  | booliano | Indica se os valores na coluna podem exceder o limite padrão de 255 caracteres.
| **columnName**            | string  | O nome da coluna de origem de pesquisa.
| **listId**                | string  | O identificador exclusivo da lista de origem de pesquisa.
| **primaryLookupColumnId** | string  | Se especificado, esta coluna é uma *pesquisa secundária*, obtendo um campo adicional da lista pesquisada pela *pesquisa primária*. Use o item da lista procurado pela pesquisa *primária* como a fonte para a coluna nomeada aqui.

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn",
  "suppressions": []
}
-->
