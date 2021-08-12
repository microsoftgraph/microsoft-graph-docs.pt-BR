---
title: Tipo de recurso resourceData
description: Representa os dados de resouce anexados à notificação de alteração enviada ao assinante.
localization_priority: Normal
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: b2be1539226ac619b15e61cc7da55d3a9c844f9a47e0e60dcf6ff80914d1a12a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54169344"
---
# <a name="resourcedata-resource-type"></a>Tipo de recurso resourceData

Namespace: microsoft.graph

Representa os dados de resouce anexados à notificação de alteração enviada ao assinante.

Para obter detalhes, confira [Usar a API do Microsoft Graph para receber notificações de alteração](webhooks.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

Para Outlook recursos, **resourceData** contém os seguintes campos:

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| @odata.type | string | O tipo de entidade OData no Microsoft Graph que descreve o objeto representado. |
| @odata.id | string | O identificador OData do objeto. |
| @odata.etag | string | A marca da entidade HTTP que representa a versão do objeto. |
| id | string | O identificador do objeto. |

> **Observação:** O `id` valor fornecido em **resourceData** é válido no momento em que a notificação de alteração foi gerada. Algumas ações, como mover uma mensagem para outra pasta, podem resultar na não validade quando a notificação `id` de alteração for processada.

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

