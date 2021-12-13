---
title: Tipo de recurso personalTaskProperties
description: Contém propriedades pessoais de uma tarefa"
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 56007de468b5fd06998b94f5b5256cfb170ba127
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424816"
---
# <a name="personaltaskproperties-resource-type"></a>Tipo de recurso personalTaskProperties

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém propriedades pessoais de uma [tarefa](task.md). Ao compartilhar ou atribuir uma **tarefa,** essas propriedades não serão vistas por outros usuários.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|reminderDatetime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data e a hora para que um alerta de lembrete da **tarefa** ocorra.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.personalTaskProperties"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personalTaskProperties",
  "reminderDatetime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  }
}
```

