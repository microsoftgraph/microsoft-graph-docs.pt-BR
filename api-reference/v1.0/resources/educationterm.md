---
title: Tipo de recurso educationTerm
description: Termo A. Isso representa uma parte designada do ano acadêmico. É usada dentro de educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 00a521ee9474d023bfcb5e72cc2e8ac45d270341a7e65ed29f920eaf33bc50f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205833"
---
# <a name="educationterm-resource-type"></a>Tipo de recurso educationTerm

Namespace: microsoft.graph

Termo A. Isso representa uma parte designada do ano acadêmico. É usada dentro de [educationClass](educationclass.md).

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo   | Descrição                       |
| :---------- | :----- | :-------------------------------- |
| displayName | Cadeia de caracteres | Nome de exibição do termo.         |
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
