---
title: tipo de recurso educationSynchronizationError
description: Representa um erro durante a validação e/ou sincronização de perfil de dados da escola. Um erro exclusivo é gerado para cada entrada que não consegue validar e/ou sincronizar com o Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d46d1160ae59174d9fcb4df89559531e3a032e55
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500321"
---
# <a name="educationsynchronizationerror-resource-type"></a>tipo de recurso educationSynchronizationError

Namespace: Microsoft. Graph

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
