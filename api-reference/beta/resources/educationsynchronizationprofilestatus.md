---
title: Tipo de recurso educationSynchronizationProfileStatus
description: 'Representa o status de sincronização de um perfil de sincronização de dados escolares. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 55636a78cd904c6992de0cf48ab333ccef8bb84a
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534190"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a>Tipo de recurso educationSynchronizationProfileStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status de sincronização de um perfil de [sincronização de](educationsynchronizationprofile.md)dados escolares.

> **Observação:** As atualizações para **educationSynchronizationProfileStatus** podem ser atrasadas devido à natureza assíncrona do processamento de sincronização em segundo plano.

## <a name="methods"></a>Métodos

| Método                                                                      | Tipo de retorno                               | Descrição                                              |
| :-------------------------------------------------------------------------- | :---------------------------------------- | :------------------------------------------------------- |
| [Obter status de uma sincronização](../api/educationsynchronizationprofilestatus-get.md) | **educationSynchronizationProfileStatus** | Retorne o status de um perfil de sincronização específico. |

## <a name="properties"></a>Propriedades

| Propriedade                    | Tipo                           | Descrição                                                                                                              |
| :-------------------------- | :----------------------------- | :----------------------------------------------------------------------------------------------------------------------- |
| id                          | String                         | O identificador exclusivo do recurso. (somente leitura)                                                                      |
| status                      | educationSynchronizationStatus | O status de uma sincronização. Os valores possíveis são: `paused` , , , , , , `inProgress` , `success` `error` `quarantined` `validationError` `extracting` *. `validating`* |
| lastSynchronizationDateTime | DateTimeOffset                 | Representa a hora da sincronização mais recente bem-sucedida.                                        |
| lastActivityDateTime | DateTimeOffset                 | Representa a hora em que as alterações mais recentes foram observadas no perfil.                                        |
| errorCount | Int                 | Número de erros durante a sincronização.                                        |
| statusMessage | Cadeia de Caracteres                 | Mensagem de status para o estágio de sincronização do perfil atual.                                        |

Os status "Extração" e "Validação" só são retornados para aplicativos preparados para lidar com novos membros de número. O opt-in é feito definindo HTTP prefer request header: `Prefer: include-unknown-enum-members` . Consulte mais sobre: [enums evolváveis](/graph/best-practices-concept#evolvable-enums).


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
  "lastSynchronizationDateTime": "DateTimeOffset",
  "lastActivityDateTime": "DateTimeOffset",
  "errorCount": "Int",
  "statusMessage": "String"
}
```
