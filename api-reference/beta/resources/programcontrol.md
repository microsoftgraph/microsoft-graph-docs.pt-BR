---
title: Tipo de recurso programControl
description: No recurso de revisões de acesso do Azure AD, o objeto de controle do programa representa um controle, vinculando uma revisão de acesso a um programa.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 492dc57bfa332472cb7565580ffaa8a5260234c0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443976"
---
# <a name="programcontrol-resource-type"></a>Tipo de recurso programControl

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de revisões de acesso do Azure [AD,](accessreviews-root.md) o objeto de controle do programa representa um controle, vinculando uma revisão de acesso a um programa.


## <a name="methods"></a>Methods

| Método | Tipo de retorno | Descrição |
|:------ |:----------- |:----------- |
| [Criar programControl](../api/programcontrol-create.md) |    [programControl](programcontrol.md) |   Adicione um programControl a um programa. |
| [Excluir programControl](../api/programcontrol-delete.md) | Nenhum. | Remova um programControl de um programa. |
| [Listar programControls](../api/programcontrol-list.md) | [Coleção programControl](programcontrol.md) | Listar controles em todos os programas no locatário. |
| [Listar programControls de um programa](../api/program-listcontrols.md) | [Coleção programControl](programcontrol.md) |    Obter uma coleção dos controles de um programa. |
| [Listar programControlTypes](../api/programcontroltype-list.md) | [Coleção programControlType](programcontroltype.md)| Listar tipos de controle de programa. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição |
|:-------- |:---- |:----------- |
| id | String | O identificador atribuído ao recurso do link entre o programa e o controle. |
| programId | String | O programId do programa do que esse controle faz parte. Obrigatório durante a criação. |
| controlId | String | ControlId do controle, em particular o identificador de uma revisão de acesso. Obrigatório durante a criação. |
| controlTypeId | String | O programControlType identifica o tipo de controle de programa - por exemplo, um controle que vincula a avaliações de acesso de convidados. Obrigatório durante a criação. |
| displayName | String | O nome do controle. |
| status | String | O status do ciclo de vida do controle. |
| createdDateTime | DateTimeOffset | A data e a hora de criação do controle do programa. |
| owner | [userIdentity](useridentity.md) | O usuário que criou o controle do programa. |
| recurso | [programResource](programresource.md) | O recurso, um grupo ou um aplicativo, direcionado pela revisão de acesso desse controle de programa. |

## <a name="relationships"></a>Relações

| Relação | Tipo   | Descrição |
|:------------ |:---- |:----------- |
| program | [program](program.md) | O programa do que esse controle faz parte. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.programControl"
}-->

```json
{
 "id": "string (identifier)",
 "programId": "string (identifier)",
 "controlId": "string (identifier)",
 "controlTypeId": "string (identifier)",
 "displayName": "string",
 "status": "string",
 "createdDateTime": "string (timestamp)",
 "owner": {"@odata.type":"microsoft.graph.userIdentity"},
 "resource":{"@odata.type":"microsoft.graph.programResource"}
}
```
<!--
{
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


