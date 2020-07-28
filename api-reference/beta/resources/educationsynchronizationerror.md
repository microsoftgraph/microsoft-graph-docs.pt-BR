---
title: tipo de recurso educationSynchronizationError
description: Representa um erro durante a validação e/ou sincronização de perfil de dados da escola. Um erro exclusivo é gerado para cada entrada que não consegue validar e/ou sincronizar com o Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 59650bc56554b9bd4dd7135ae44d53e153c159f8
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434834"
---
# <a name="educationsynchronizationerror-resource-type"></a>tipo de recurso educationSynchronizationError

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um erro durante a validação e/ou sincronização de perfil de dados da escola. Um erro exclusivo é gerado para cada entrada que não consegue validar e/ou sincronizar com o Azure Active Directory (Azure AD).

## <a name="methods"></a>Métodos

| Método                                                                     | Tipo de retorno                                  | Descrição                                                           |
| :------------------------------------------------------------------------- | :------------------------------------------- | :-------------------------------------------------------------------- |
| [Obter erros de sincronização](../api/educationsynchronizationerrors-get.md) | coleção **educationSynchronizationError** | Retorna a lista de erros de sincronização associados a um perfil. |

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo           | Descrição                                                     |
| :------------------- | :------------- | :-------------------------------------------------------------- |
| id                   | Cadeia de caracteres         | O identificador exclusivo do recurso. (somente leitura)             |
| EntryType            | Cadeia de caracteres         | Representa a entidade de sincronização (escola, seção, aluno, professor). |
| errorCode            | Cadeia de caracteres         | Representa o código de erro para esse erro.                       |
| errorMessage         | Cadeia de caracteres         | Contém uma descrição do erro.                            |
| unindovalue         | Cadeia de caracteres         | O identificador exclusivo da entrada.                            |
| recordedDateTime     | DateTimeOffset | A hora da ocorrência desse erro.                           |
| reportableIdentifier | Cadeia de caracteres         | O identificador desta entrada de erro.                             |

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
