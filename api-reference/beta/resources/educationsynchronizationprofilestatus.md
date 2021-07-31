---
title: Tipo de recurso educationSynchronizationProfileStatus
description: 'Representa o status de sincronização de um perfil de sincronização de dados escolares. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ee802e9749418b9a1d2a9bbdbe3916493e5cf431
ms.sourcegitcommit: 596b3d5636f3f3e042d180ea8f039f00ebd6b38a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2021
ms.locfileid: "53665904"
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
| id                          | Cadeia de caracteres                         | O identificador exclusivo do recurso. (somente leitura)                                                                      |
| status                      | educationSynchronizationStatus | O status de uma sincronização. Os valores possíveis são: `paused` , , , , , , , , `inProgress` , `success` `error` `validationError` `quarantined` `unknownFutureValue` `extracting` `validating` . Observe que você deve usar o header de solicitação para obter os seguintes valores neste `Prefer: include-unknown-enum-members` [número evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `extracting` , `validating` .|
| lastSynchronizationDateTime | DateTimeOffset                 | Representa a hora da sincronização mais recente bem-sucedida.                                        |
| lastActivityDateTime | DateTimeOffset                 | Representa a hora em que as alterações mais recentes foram observadas no perfil.                                        |
| errorCount | Int                 | Número de erros durante a sincronização.                                        |
| statusMessage | Cadeia de caracteres                 | Mensagem de status para o estágio de sincronização do perfil atual.                                        |


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
