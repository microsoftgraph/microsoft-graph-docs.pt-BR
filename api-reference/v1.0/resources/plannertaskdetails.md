---
title: Tipo de recurso plannerTaskDetails
description: O **recurso plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto de tarefa tem um objeto details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 852deda3e48c78b2e70968cb7e8b7ec9a11956bbf2fcab66ecc127ea653abce9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189391"
---
# <a name="plannertaskdetails-resource-type"></a>Tipo de recurso plannerTaskDetails

Namespace: microsoft.graph

O **recurso plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada [objeto de](plannertask.md) tarefa tem um objeto details.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter plannerTaskDetails](../api/plannertaskdetails-get.md) | [plannerTaskDetails](plannertaskdetails.md) |Ler propriedades e relações do **objeto plannerTaskDetails.**|
|[Atualizar](../api/plannertaskdetails-update.md) | [plannerTaskDetails](plannertaskdetails.md)    |Atualize **o objeto plannerTaskDetails.** |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|checklist|[plannerChecklistItems](plannerchecklistitems.md)|A coleção de itens de lista de verificação na tarefa.|
|description|Cadeia de caracteres|Descrição da tarefa|
|id|String| Somente leitura. ID dos detalhes da tarefa. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.|
|previewType|string|Isso define o tipo de visualização que aparece na tarefa. Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Quando definido para `automatic` a visualização exibida, é escolhido pelo aplicativo exibindo a tarefa.|
|referências|[plannerExternalReferences](plannerexternalreferences.md)|A coleção de referências na tarefa.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

