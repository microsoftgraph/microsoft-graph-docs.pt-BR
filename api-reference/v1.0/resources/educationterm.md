---
title: Tipo de recurso educationTerm
description: Termo A. Isso representa uma parte designada do ano acadêmico. É usada dentro de educationClass.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 792f490ef9aa8ccdf6155b0eee0daf9f7c66b3b9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118663"
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
