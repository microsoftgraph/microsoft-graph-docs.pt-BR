---
title: tipo de recurso de educationSynchronizationProfileStatus
description: 'Representa o status da sincronização de um perfil de sincronização de dados escola. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d16619b0cf1e2c09358cf585b896b0c7c7d4f318
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928924"
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
