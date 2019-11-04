---
title: tipo de recurso educationalActivity
description: tipo de recurso educationalActivity
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 8d060de55d765adb7e01e6b03842c569f03c8d4f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939618"
---
# <a name="educationalactivity-resource-type"></a>tipo de recurso educationalActivity

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os dados que um usuário forneceu relacionados ao Undergraduate, graduado, dograduação ou outras atividades educacionais.

Herda as propriedades de metadados de [Myfacet](itemfacet.md).

## <a name="methods"></a>Métodos

| Método                                                       | Tipo de retorno                                   | Descrição                                                      |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [Obter educationalActivity](../api/educationalactivity-get.md) | [educationalActivity](educationalactivity.md) | Leia as propriedades e os relacionamentos do objeto educationalActivity. |
| [Update](../api/educationalactivity-update.md)               | [educationalActivity](educationalactivity.md) | Atualize o objeto educationalActivity.                               |
| [Delete](../api/educationalactivity-delete.md)               | None                                          | Exclua o objeto educationalActivity.                               |

## <a name="properties"></a>Propriedades

| Propriedade           | Tipo                                                      | Descrição                                                                |
|:-------------------|:----------------------------------------------------------|:---------------------------------------------------------------------------|
|completionMonthYear |Data                                                       |O mês e o ano em que o usuário formou ou concluiu a atividade.            |
|endMonthYear        |Data                                                       |O mês e o ano em que o usuário concluiu a atividade educacional referenciada.  |
|instituição         |[institutionData](institutiondata.md)                      |Contém detalhes da instituição estudada em.                             |
|programa             |[educationalActivityDetail](educationalactivitydetail.md)  |Contém informações estendidas sobre o programa ou o curso.                  |
|startMonthYear      |Data                                                       |O mês e o ano em que o usuário tiver iniciado a atividade referenciada.              |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationalActivity",
  "baseType": ""
}-->

```json
{
  "completionMonthYear": "String (timestamp)",
  "endMonthYear": "String (timestamp)",
  "institution": {"@odata.type": "microsoft.graph.institutionData"},
  "program": {"@odata.type": "microsoft.graph.educationalActivityDetail"},
  "startMonthYear": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationalActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->