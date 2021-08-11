---
title: Tipo de recurso scheduleInformation
description: Representa a disponibilidade de um usuário, lista de distribuição ou recurso para um período de tempo especificado.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 67b7396cfebc19baa3771c2ec8d153950928288506cfc699851b891e15409a0f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54231478"
---
# <a name="scheduleinformation-resource-type"></a>Tipo de recurso scheduleInformation

Namespace: microsoft.graph

Representa a disponibilidade de um usuário, lista de distribuição ou recurso (sala ou equipamento) por um período de tempo especificado.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|availabilityView |Cadeia de caracteres |Representa uma exibição mesclada de disponibilidade de todos os itens em `scheduleItems` . A exibição consiste em intervalos de tempo. A disponibilidade durante cada intervalo de tempo é indicada com: `0` = livre, `1` = provisório, = ocupado, = sem `2` `3` escritório, = trabalhando em outro `4` lugar.|
|erro |[freeBusyError](freebusyerror.md) |Informações de erro da tentativa de obter a disponibilidade do usuário, lista de distribuição ou recurso. |
|scheduleId |Cadeia de caracteres |Um endereço SMTP do usuário, lista de distribuição ou recurso, identificando uma instância de **scheduleInformation**. |
|scheduleItems |[Coleção scheduleItem](scheduleitem.md) |Contém os itens que descrevem a disponibilidade do usuário ou do recurso. |
|workingHours |[workingHours](workinghours.md) |Os dias da semana e as horas de um fuso horário específico que o usuário trabalha. Eles são definidos como parte das caixas de [correio do usuárioSettings](mailboxsettings.md).|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleInformation"
}-->

```json
{
  "availabilityView": "String",
  "error": {"@odata.type": "microsoft.graph.freeBusyError"},
  "scheduleId": "String",
  "scheduleItems": [{"@odata.type": "microsoft.graph.scheduleItem"}],
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->

