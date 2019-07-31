---
title: tipo de recurso businessFlowTemplate
description: No recurso de revisões do Azure AD Access, `businesFlowTemplate` o representa um modelo de fluxo de negócios do Azure AD. O identificador de um modelo, como a análise de membros convidados de um grupo, é fornecido pelo chamador durante a criação de uma revisão do Access.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6890ed724c1a71c69a881ce0e2e70675b3537520
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973481"
---
# <a name="businessflowtemplate-resource-type"></a>tipo de recurso businessFlowTemplate

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de revisões do Azure AD [Access](accessreviews-root.md) , `businesFlowTemplate` o representa um modelo de fluxo de negócios do Azure AD. O identificador de um modelo, como a análise de membros convidados de um grupo, é fornecido pelo chamador durante a criação de uma revisão do Access.

Os objetos do modelo de fluxo de negócios são gerados automaticamente quando o administrador global embuti o locatário para usar o recurso de revisões do Access.  Nenhum modelo de fluxo de negócios adicional pode ser criado.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar businessFlowTemplates](../api/businessflowtemplate-list.md) | coleção [businessFlowTemplate](businessflowtemplate.md)| Obtenha os modelos de fluxo de negócios apropriados para as revisões do Access.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `id`                     |`String`                | O identificador atribuído ao recurso do modelo de fluxo de negócios                                      |
| `displayName`            |`String`                | O nome do modelo de fluxo de negócios                                                             |


## <a name="relationships"></a>Relações

Nenhum

## <a name="see-also"></a>Ver também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Criar um novo accessReview. |


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.businessFlowTemplate"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "businessFlowTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
