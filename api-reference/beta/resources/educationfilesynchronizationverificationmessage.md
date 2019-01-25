---
title: tipo de recurso de educationFileSynchronizationVerificationMessage
description: Representa um erro retornado ao cliente em resposta a uma solicitação para iniciar a sincronização de perfis de dados baseada em CSV escola. O recurso irá conter erros resultantes da verificação. Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (AD Azure).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 26f96c83ce14539011664b446265328f714ed402
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529891"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a>tipo de recurso de educationFileSynchronizationVerificationMessage

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um erro retornado ao cliente em resposta a uma solicitação para [Iniciar a sincronização](../api/educationsynchronizationprofile-start.md) de perfis de dados baseada em CSV escola. O recurso irá conter erros resultantes da verificação. Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (AD Azure).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **type** | string | Tipo da mensagem. Os valores possíveis são: `error`, `warning`, `information`. | 
| **fileName** | string | Arquivo de origem que contém o erro. |
| **description** | string | Informações detalhadas sobre o tipo de mensagem. |

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfilesynchronizationverificationmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
