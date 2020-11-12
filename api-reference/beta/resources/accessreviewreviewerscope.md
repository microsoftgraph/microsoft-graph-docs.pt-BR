---
title: tipo de recurso accessReviewReviewerScope
description: Representa quem irá revisar uma revisão do Access.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: edc25e19a51f787dd0799fbd9e6e6c2a1b45787e
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000775"
---
# <a name="accessreviewreviewerscope-resource-type"></a>tipo de recurso accessReviewReviewerScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O accessReviewReviewerScope define quem irá revisar instâncias de um [accessReviewScheduleDefinition](accessreviewscheduledefinition.md). Isso é expresso como uma consulta OData, que permite que os revisores sejam especificados como uma lista estática de usuários (ou seja, usuários específicos, proprietários de grupo, membros do grupo) ou dinamicamente (ou seja, o caso em que cada usuário é revisado por seu gerente). Para criar uma autoanálise (onde os usuários revisam seu próprio acesso), não forneça revisores na criação do [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) .


## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :-------------------------| :---------- | :---------- |
| consulta | Cadeia de caracteres | A consulta especificando quem será o revisor. Consulte a tabela para obter exemplos. |
| queryType | Cadeia de caracteres | O tipo de consulta. Os exemplos incluem `MicrosoftGraph` e `ARM` . |
| queryRoot | Cadeia de caracteres | No cenário em que os revisores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a fonte relativa da consulta. Essa propriedade só será necessária se uma consulta relativa (ou seja,./Manager) for especificada. |

### <a name="supported-queries-for-accessreviewreviewerscope"></a>Consultas com suporte para o accessReviewReviewerScope

|Cenário| consulta | queryType | queryRoot |
|--|--|--|--|
| Proprietário do grupo como revisor | /groups/{Group ID}/Owners |MicrosoftGraph||
| Usuário específico como revisor | ID/Users/{User} |MicrosoftGraph||
| Gerente do usuário que está sendo revisado como revisor | ./manager | MicrosoftGraph |correta|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewReviewerScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewReviewerScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewReviewerScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
