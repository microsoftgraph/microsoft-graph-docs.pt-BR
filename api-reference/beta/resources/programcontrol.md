---
title: Tipo de recurso programControl (preterido)
description: No recurso Azure AD revisões de acesso, o objeto de controle de programa representa um controle, vinculando uma revisão de acesso a um programa.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 8f3acee6e81452f9cc5cc839ab89b5ee61cfa401
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820914"
---
# <a name="programcontrol-resource-type-deprecated"></a>Tipo de recurso programControl (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

No recurso Azure AD [revisões de acesso](accessreviews-root.md), o objeto de controle de programa representa um controle, vinculando uma revisão de acesso a um programa.


## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:------ |:----------- |:----------- |
| [Criar programControl](../api/programcontrol-create.md) |    [programControl](programcontrol.md) |   Adicione um programControl a um programa. |
| [Excluir programControl](../api/programcontrol-delete.md) | Nenhum | Remova um programControl de um programa. |
| [Listar programControls](../api/programcontrol-list.md) | [coleção programControl](programcontrol.md) | Listar controles em todos os programas no locatário. |
| [Listar programControls de um programa](../api/program-listcontrols.md) | [coleção programControl](programcontrol.md) |    Obtenha uma coleção dos controles de um programa. |
| [Listar programControlTypes](../api/programcontroltype-list.md) | [coleção programControlType](programcontroltype.md)| Listar tipos de controle de programa. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição |
|:-------- |:---- |:----------- |
| id | Cadeia de caracteres | O identificador atribuído pelo recurso do link entre o programa e o controle. |
| programId | Cadeia de caracteres | A programId do programa do que esse controle faz parte. Obrigatório durante a criação. |
| Controlid | Cadeia de caracteres | A controlId do controle, em particular o identificador de uma revisão de acesso. Obrigatório durante a criação. |
| controlTypeId | Cadeia de caracteres | O programControlType identifica o tipo de controle de programa – por exemplo, um controle vinculado a revisões de acesso de convidado. Obrigatório durante a criação. |
| displayName | Cadeia de caracteres | O nome do controle. |
| status | String | O status do ciclo de vida do controle. |
| createdDateTime | DateTimeOffset | A data e hora de criação do controle do programa. |
| owner | [userIdentity](useridentity.md) | O usuário que criou o controle do programa. |
| recurso | [programResource](programresource.md) | O recurso, um grupo ou um aplicativo, direcionado pela revisão de acesso desse controle de programa. |

## <a name="relationships"></a>Relações

| Relação | Tipo   | Descrição |
|:------------ |:---- |:----------- |
| Programa | [Programa](program.md) | O programa do que esse controle faz parte. |

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


