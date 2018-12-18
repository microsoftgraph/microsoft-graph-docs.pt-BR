---
title: tipo de recurso de educationSynchronizationError
description: Representa um erro durante a validação de perfil de dados escola e/ou de sincronização. Será gerado um erro de exclusivo para cada entrada que está falhando para validar e/ou sincronizar com o Azure Active Directory (AD Azure).
author: mmast-msft
ms.openlocfilehash: d950e906a506c3cf1ee5bc5b627200dc79c1d0fb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335998"
---
# <a name="educationsynchronizationerror-resource-type"></a>tipo de recurso de educationSynchronizationError

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um erro durante a validação de perfil de dados escola e/ou de sincronização. Será gerado um erro de exclusivo para cada entrada que está falhando para validar e/ou sincronizar com o Azure Active Directory (AD Azure).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-|:-|:-|
| [Obtenha os erros de sincronização](../api/educationsynchronizationerrors-get.md) | coleção **educationSynchronizationError**| Retorna a lista de erros de sincronização associado a um perfil. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **entryType** | string |  Representa a entidade de sincronização (escola, seção, estudante, professor).       |
| **errorCode** | string |  Representa o código de erro para esse erro.         |
| **errorMessage** | string |  Contém uma descrição do erro.        |
| **joiningValue** | string |  O identificador exclusivo para a entrada.         |
| **recordedDateTime** | DateTimeOffset | A hora da ocorrência desse erro.         |
| **reportableIdentifier** | string | O identificador dessa entrada de erro.       |

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationError"
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
