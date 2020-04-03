---
title: tipo de recurso programControl
description: No recurso de revisões do Azure AD Access, o objeto de controle do programa representa um controle, vinculando uma revisão do Access a um programa.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 3cc26caaee20f1f274265061139671d00fa7cee0
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125306"
---
# <a name="programcontrol-resource-type"></a>tipo de recurso programControl

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de revisões do Azure AD [Access](accessreviews-root.md) , o objeto de controle do programa representa um controle, vinculando uma revisão do Access a um programa.


## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Adicionar um programControl a um programa.|
|[Excluir programControl](../api/programcontrol-delete.md) |     Nenhum.   |   Remover um programControl de um programa.|
|[Listar programControls](../api/programcontrol-list.md) | coleção [programControl](programcontrol.md)| Listar controles em todos os programas no locatário.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `id`                     |`String`                | O identificador atribuído ao recurso do link entre o programa e o controle                                      |
| `programId`              |`String`                | O ProgramId do programa do qual esse controle faz parte. Obrigatório ao criar.                            |
| `controlId`              |`String`                | O controlId do controle, em particular, o identificador de uma revisão do Access. Obrigatório ao criar.                                                |
| `controlTypeId`          |`String`                | O programControlType identifica o tipo de controle de programa-por exemplo, um controle vinculando a revisões de acesso de convidados. Obrigatório ao criar. |
| `displayName`            |`String`                | O nome do controle.                                                             |
| `status`                 |`String`                | O status do ciclo de vida do controle.                                                 |
| `createdDateTime`        |`DateTimeOffset`        | A data e hora de criação do controle de programa.                                        |
| `owner`                  |[userIdentity](useridentity.md)   | O usuário que criou o controle de programa.                                               |
| `resource`               |`programResource`       | O recurso, um grupo ou um aplicativo, direcionado por essa revisão de acesso de controle de programa.                   |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `program`                |[programa](program.md)               | O programa do qual esse controle faz parte.                                                |

## <a name="see-also"></a>Confira também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar programControls de um programa](../api/program-listcontrols.md) |      coleção [programControl](programcontrol.md)| Obter uma coleção de controles de um programa.|
|[Listar programControlTypes](../api/programcontroltype-list.md) | coleção [programControlType](programcontroltype.md)| Listar tipos de controle de programa. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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

## <a name="the-programresource-complex-type"></a>O tipo complexo programResource

O recurso de programa, contido em um objeto de controle de programa, é uma representação de uma referência a um objeto que é o destino da revisão do Access.

Este tipo herda de `microsoft.graph.identity` e tem uma propriedade adicional:

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `type`               |`String`  | Tipo do recurso, indicando se é um grupo ou um aplicativo. |     

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programResource"
}-->

```json
{
 "type": "string"
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
