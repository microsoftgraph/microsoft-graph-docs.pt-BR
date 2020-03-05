---
title: tipo de recurso educationSynchronizationProfileStatus
description: 'Representa o status de sincronização de um perfil de sincronização de dados da escola. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 88e2f85cc4b24bd55cdfc1fbc5aeecd7bee8c461
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500027"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a>tipo de recurso educationSynchronizationProfileStatus

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status de sincronização de um [perfil de sincronização](educationsynchronizationprofile.md)de dados da escola. 

> **Observação:** As atualizações do **educationSynchronizationProfileStatus** podem ser atrasadas devido à natureza assíncrona do processamento de sincronização em segundo plano.

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-|:-|:-|
| [Obter o status de uma sincronização](../api/educationsynchronizationprofilestatus-get.md) | **educationSynchronizationProfileStatus** | Retornar o status de um perfil de sincronização específico. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **status** | educationSynchronizationStatus | O status de uma sincronização. Os valores possíveis são `paused`: `inProgress`, `success`, `error`, `quarantined`, `validationError`,. |
| **lastSynchronizationDateTime** | DateTimeOffset | Representa a hora em que as alterações mais recentes foram observadas no diretório.  |

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```
