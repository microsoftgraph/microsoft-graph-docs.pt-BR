---
title: tipo de recurso de businessFlowTemplate
description: No Windows Azure AD access analisa o recurso, o `businesFlowTemplate` representa um modelo de fluxo de negócios do Azure AD. O identificador de um modelo, por exemplo, para revisar os membros de convidado de um grupo, é fornecido pelo chamador ao criar uma revisão de acesso.
localization_priority: Normal
ms.openlocfilehash: 567a7f499e2fb493f3ca519e312e69fb43fe3b79
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529576"
---
# <a name="businessflowtemplate-resource-type"></a>tipo de recurso de businessFlowTemplate

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de [acesso analisa](accessreviews-root.md) Azure AD, o `businesFlowTemplate` representa um modelo de fluxo de negócios do Azure AD. O identificador de um modelo, por exemplo, para revisar os membros de convidado de um grupo, é fornecido pelo chamador ao criar uma revisão de acesso.

Os objetos de modelo de fluxo de negócios são gerados automaticamente quando o onboards administrador global locatário para usar o access revisa o recurso.  Nenhum modelo de fluxo de negócios adicionais pode ser criado.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Lista businessFlowTemplates](../api/businessflowtemplate-list.md) | coleção [businessFlowTemplate](businessflowtemplate.md)| Obtenha os modelos de fluxo de negócios apropriado para acessar as revisões.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `id`                     |`String`                | O identificador atribuído pelo recurso de modelo de fluxo de negócio                                      |
| `displayName`            |`String`                | O nome do modelo de fluxo de negócio                                                             |


## <a name="relationships"></a>Relações

Nenhum.

## <a name="see-also"></a>Ver também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Crie um novo accessReview. |


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
  "suppressions": [
    "Error: /api-reference/beta/resources/businessflowtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
