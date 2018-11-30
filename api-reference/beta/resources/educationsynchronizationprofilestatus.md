---
title: tipo de recurso de educationSynchronizationProfileStatus
description: 'Representa o status da sincronização de um perfil de sincronização de dados escola. '
ms.openlocfilehash: 6d2c638e1f92a6c3e090cb2bf3bb55e8482bbc4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040945"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a>tipo de recurso de educationSynchronizationProfileStatus

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa o status da sincronização de um [perfil de sincronização](educationsynchronizationprofile.md)de dados do escola. 

> **Observação:** Atualizações para o **educationSynchronizationProfileStatus** podem ser atrasadas devido a natureza assíncrona do processamento de sincronização em segundo plano.

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-|:-|:-|
| [Obter o status de uma sincronização](../api/educationsynchronizationprofilestatus-get.md) | **educationSynchronizationProfileStatus** | Retorna o status de um perfil de sincronização específico. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **status** | string | O status de uma sincronização. Os valores possíveis são: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`. |
| **lastSynchronizationDateTime** | DateTimeOffset | Representa a hora quando as alterações mais recentes têm foi observadas no diretório.  |

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```