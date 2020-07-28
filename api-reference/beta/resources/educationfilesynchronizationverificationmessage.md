---
title: tipo de recurso educationFileSynchronizationVerificationMessage
description: Representa um erro retornado ao cliente em resposta a uma solicitação para iniciar a sincronização de perfis de dados escolares baseados em CSV. O recurso conterá erros resultantes da verificação. Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8e82ede1df5c17b99fdc40857fd97f1f90012711
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434974"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a>tipo de recurso educationFileSynchronizationVerificationMessage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um erro retornado ao cliente em resposta a uma solicitação para [iniciar a sincronização](../api/educationsynchronizationprofile-start.md) de perfis de dados escolares baseados em CSV. O recurso conterá erros resultantes da verificação. Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (Azure AD).

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo   | Descrição                                                                  |
| :---------- | :----- | :--------------------------------------------------------------------------- |
| type        | string | Tipo da mensagem. Os valores possíveis são: `error`, `warning`, `information`. |
| nomes    | cadeia de caracteres | Arquivo de origem que contém o erro.                                         |
| description | string | Informações detalhadas sobre o tipo de mensagem.                                 |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage"
}-->

```json
{
  "type": "String",
  "fileName": "String",
  "description": "String"
}
```
