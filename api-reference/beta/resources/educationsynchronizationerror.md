---
title: tipo de recurso educationSynchronizationError
description: Representa um erro durante a validação e/ou sincronização de perfil de dados da escola. Um erro exclusivo é gerado para cada entrada que não consegue validar e/ou sincronizar com o Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2af4ef9f17452714373d42b67af6e87a7f87fe1d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989644"
---
# <a name="educationsynchronizationerror-resource-type"></a>tipo de recurso educationSynchronizationError

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um erro durante a validação e/ou sincronização de perfil de dados da escola. Um erro exclusivo é gerado para cada entrada que não consegue validar e/ou sincronizar com o Azure Active Directory (Azure AD).

## <a name="methods"></a>Methods

| Método                                                                     | Tipo de retorno                                  | Descrição                                                           |
| :------------------------------------------------------------------------- | :------------------------------------------- | :-------------------------------------------------------------------- |
| [Obter erros de sincronização](../api/educationsynchronizationerrors-get.md) | coleção **educationSynchronizationError** | Retorna a lista de erros de sincronização associados a um perfil. |

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo           | Descrição                                                     |
| :------------------- | :------------- | :-------------------------------------------------------------- |
| id                   | String         | O identificador exclusivo do recurso. (somente leitura)             |
| EntryType            | String         | Representa a entidade de sincronização (escola, seção, aluno, professor). |
| errorCode            | Cadeia de caracteres         | Representa o código de erro para esse erro.                       |
| errorMessage         | String         | Contém uma descrição do erro.                            |
| unindovalue         | String         | O identificador exclusivo da entrada.                            |
| recordedDateTime     | DateTimeOffset | A hora da ocorrência desse erro.                           |
| reportableIdentifier | String         | O identificador desta entrada de erro.                             |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationError"
}-->

```json
{
  "id": "String",
  "entryType": "String",
  "errorCode": "String",
  "errorMessage": "String",
  "joiningValue": "String",
  "recordedDateTime": "DateTimeOffset",
  "reportableIdentifier": "String"
}
```


