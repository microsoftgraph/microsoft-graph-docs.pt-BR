---
title: tipo de recurso educationSynchronizationProfileStatus
description: 'Representa o status de sincronização de um perfil de sincronização de dados da escola. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2ba9b9d8ecf6766cddfa670ae2e33b39d0e6acb6
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434869"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a>tipo de recurso educationSynchronizationProfileStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status de sincronização de um [perfil de sincronização](educationsynchronizationprofile.md)de dados da escola.

> **Observação:** As atualizações do **educationSynchronizationProfileStatus** podem ser atrasadas devido à natureza assíncrona do processamento de sincronização em segundo plano.

## <a name="methods"></a>Métodos

| Método                                                                      | Tipo de retorno                               | Descrição                                              |
| :-------------------------------------------------------------------------- | :---------------------------------------- | :------------------------------------------------------- |
| [Obter o status de uma sincronização](../api/educationsynchronizationprofilestatus-get.md) | **educationSynchronizationProfileStatus** | Retornar o status de um perfil de sincronização específico. |

## <a name="properties"></a>Propriedades

| Propriedade                    | Tipo                           | Descrição                                                                                                              |
| :-------------------------- | :----------------------------- | :----------------------------------------------------------------------------------------------------------------------- |
| id                          | Cadeia de caracteres                         | O identificador exclusivo do recurso. (somente leitura)                                                                      |
| status                      | educationSynchronizationStatus | O status de uma sincronização. Os valores possíveis são: `paused` , `inProgress` , `success` , `error` , `quarantined` , `validationError` . |
| lastSynchronizationDateTime | DateTimeOffset                 | Representa a hora em que as alterações mais recentes foram observadas no diretório.                                        |

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
  "id": "String",
  "status": { "@odata.type": "microsoft.graph.educationSynchronizationStatus" },
  "lastSynchronizationDateTime": "DateTimeOffset"
}
```
