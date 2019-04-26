---
title: tipo de recurso educationSynchronizationError
description: Representa um erro durante a validação e/ou sincronização de perfil de dados da escola. Um erro exclusivo é gerado para cada entrada que não consegue validar e/ou sincronizar com o Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3c512f921e77468bb30e5109eec29afa9b395b7e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340507"
---
# <a name="educationsynchronizationerror-resource-type"></a>tipo de recurso educationSynchronizationError

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um erro durante a validação e/ou sincronização de perfil de dados da escola. Um erro exclusivo é gerado para cada entrada que não consegue validar e/ou sincronizar com o Azure Active Directory (Azure AD).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-|:-|:-|
| [Obter erros de sincronização](../api/educationsynchronizationerrors-get.md) | coleção **educationSynchronizationError**| Retorna a lista de erros de sincronização associados a um perfil. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **EntryType** | string |  Representa a entidade de sincronização (escola, seção, aluno, professor).       |
| **errorCode** | string |  Representa o código de erro para esse erro.         |
| **errorMessage** | string |  Contém uma descrição do erro.        |
| **unindovalue** | string |  O identificador exclusivo da entrada.         |
| **recordedDateTime** | DateTimeOffset | A hora da ocorrência desse erro.         |
| **reportableIdentifier** | string | O identificador desta entrada de erro.       |

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationError"
}-->

```json
{
    "entryType": "String",
    "errorCode": "String",
    "errorMessage": "String",
    "joiningValue": "String",
    "recordedDateTime": "DateTimeOffset",
    "reportableIdentifier": "String"
}
```
