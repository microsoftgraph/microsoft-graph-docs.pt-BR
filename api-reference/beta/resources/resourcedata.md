---
title: tipo de recurso resourceData
description: Representa os dados de recursos anexados à notificação de alteração enviada ao Assinante.
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 94af6ae2c8ed1cfa9ec9c66502d48b5eabcb482f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087632"
---
# <a name="resourcedata-resource-type"></a>tipo de recurso resourceData

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os dados de recursos anexados à notificação de alteração enviada ao Assinante.

Para obter detalhes, consulte [usar a API do Microsoft Graph para obter notificações de alteração](webhooks.md).

## <a name="methods"></a>Métodos

Nenhum

## <a name="properties"></a>Propriedades

Para recursos do Outlook, **resourceData** contém os seguintes campos:

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| @odata.type | string | O tipo de entidade OData no Microsoft Graph que descreve o objeto representado. |
| @odata.id | string | O identificador OData do objeto. |
| @odata.etag | string | A marca da entidade HTTP que representa a versão do objeto. |
| id | string | O identificador do objeto. |

> **Observação:** O `id` valor fornecido em **resourceData** é válido no momento em que a notificação de alteração foi gerada. Algumas ações, como mover uma mensagem para outra pasta podem resultar na `id` não mais ser válida quando a notificação de alteração for processada.

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceData"
}-->

```json
{
  "id": "1565293727947",
  "@odata.type": "#Microsoft.Graph.ChatMessage",
  "@odata.id": "teams('88cbc8fc-164b-44f0-b6a6-b59b4a1559d3')/channels('19:8d9da062ec7647d4bb1976126e788b47@thread.tacv2')/messages('1565293727947')/replies('1565293727947')"
}
```

<!-- uuid: eb6c98ec-8257-4826-910e-5c603265257f
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "change notification resource data resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


