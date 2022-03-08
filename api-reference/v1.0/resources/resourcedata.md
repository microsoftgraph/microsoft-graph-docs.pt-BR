---
title: Tipo de recurso resourceData
description: Representa os dados de resouce anexados à notificação de alteração enviada ao assinante.
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: c8cb63331cdd2252f40eef8be468499832bca9d6
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333642"
---
# <a name="resourcedata-resource-type"></a>Tipo de recurso resourceData

Namespace: microsoft.graph

Representa os dados de recurso anexados à notificação de alteração enviada ao assinante. Esse recurso é um tipo aberto e permite que outras propriedades sejam passadas.

Para obter detalhes, confira [Usar a API do Microsoft Graph para receber notificações de alteração](webhooks.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum, exceto Outlook recursos **em que resourceData** contém os seguintes campos:

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| @odata.type | String | O tipo de entidade OData no Microsoft Graph que descreve o objeto representado. |
| @odata.id | String | O identificador OData do objeto. |
| @odata.etag | String | A marca da entidade HTTP que representa a versão do objeto. |
| id | String | O identificador do objeto. |

> **Observação:** O **valor de id** fornecido **em resourceData** é válido no momento em que a notificação de alteração foi gerada. Algumas ações, como mover uma mensagem para outra pasta, `id` podem resultar na não validade quando a notificação de alteração for processada.

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "@odata.type",
    "@odata.id",
    "@odata.etag",
    "id"
  ],
  "@odata.type": "microsoft.graph.resourceData"
}-->

```json
{
  "@odata.type": "#microsoft.graph.resourceData"
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

