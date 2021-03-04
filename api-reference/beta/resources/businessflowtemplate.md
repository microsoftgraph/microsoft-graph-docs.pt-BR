---
title: Tipo de recurso businessFlowTemplate
description: No recurso de revisões de acesso do Azure AD, o representa um modelo de fluxo de negócios do `businesFlowTemplate` Azure AD. O identificador de um modelo, como para revisar membros convidados de um grupo, é fornecido pelo chamador ao criar uma revisão de acesso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 95a2723ee20777989ed1576d02c69adc649555ed
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433142"
---
# <a name="businessflowtemplate-resource-type"></a>Tipo de recurso businessFlowTemplate

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de revisões de acesso do Azure [AD,](accessreviews-root.md) o representa um modelo de fluxo de negócios do `businesFlowTemplate` Azure AD. O identificador de um modelo, como para revisar membros convidados de um grupo, é fornecido pelo chamador ao criar uma revisão de acesso.

Os objetos do modelo de fluxo de negócios são gerados automaticamente quando o administrador global integra o locatário para usar o recurso de revisão de acesso.  Os modelos de fluxo de negócios incluem revisões de acesso de atribuições a um aplicativo, associações de um grupo, associações de uma função do Azure AD, associações de usuários convidados de um grupo e atribuições de usuário convidado a um aplicativo. Nenhum modelo de fluxo comercial adicional pode ser criado.


## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar businessFlowTemplates](../api/businessflowtemplate-list.md) | [Coleção businessFlowTemplate](businessflowtemplate.md)| Obter os modelos de fluxo de negócios apropriados para acessar avaliações.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `id`                     |`String`                | O identificador atribuído ao recurso do modelo de fluxo de negócios. Esses valores são sensíveis a minúsculas.                                      |
| `displayName`            |`String`                | O nome do modelo de fluxo comercial                                                             |


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


