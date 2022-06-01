---
title: Tipo de recurso businessFlowTemplate (preterido)
description: No recurso Azure AD revisões de acesso, ele representa `businesFlowTemplate` um Azure AD de fluxo de negócios. O identificador de um modelo, como examinar membros convidados de um grupo, é fornecido pelo chamador ao criar uma revisão de acesso.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: cfcb1cdc6997cb9b09f2f94a603a2a70c1aaf9d9
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821019"
---
# <a name="businessflowtemplate-resource-type-deprecated"></a>Tipo de recurso businessFlowTemplate (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

No recurso Azure AD [revisões de acesso](accessreviews-root.md), **o businesFlowTemplate** representa um Azure AD de fluxo de negócios. O identificador de um modelo, como examinar membros convidados de um grupo, é fornecido pelo chamador ao criar uma revisão de acesso.

Os objetos de modelo de fluxo de negócios são gerados automaticamente quando o administrador global integra o locatário para usar o recurso de revisões de acesso.  Os modelos de fluxo de negócios incluem revisões de acesso de atribuições a um aplicativo, associações de um grupo, associações de uma função Azure AD, associações de usuário convidado de um grupo e atribuições de usuário convidado a um aplicativo. Nenhum modelo de fluxo de negócios adicional pode ser criado.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar businessFlowTemplates](../api/businessflowtemplate-list.md) | [coleção businessFlowTemplate](businessflowtemplate.md)| Obtenha os modelos de fluxo de negócios apropriados para acessar revisões.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| id                     |String                | O identificador atribuído ao recurso do modelo de fluxo de negócios. Esses valores diferenciam maiúsculas de minúsculas.                                      |
| displayName            |Cadeia de caracteres                | O nome do modelo de fluxo de negócios                                                             |


## <a name="relationships"></a>Relações

Nenhum

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
  "suppressions": []
}
-->


