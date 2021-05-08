---
title: Tipo de recurso educationTerm
description: Termo A. Isso representa uma parte designada do ano acadêmico. É usada dentro de educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 41a878f58736f608cf9cc9f0c45867bf48669b1a
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231833"
---
# <a name="educationterm-resource-type"></a>Tipo de recurso educationTerm

Namespace: microsoft.graph

Termo A. Isso representa uma parte designada do ano acadêmico. É usada dentro de [educationClass](educationclass.md).

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo   | Descrição                       |
| :---------- | :----- | :-------------------------------- |
| displayName | String | Nome de exibição do termo.         |
| externalId  | Cadeia de caracteres | ID do termo no sistema de sincronização. |
| startDate   | Data   | Início do termo.                |
| endDate     | Data   | Fim do termo.                  |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationTerm"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationTerm",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date",
  "displayName": "String"
}
```
