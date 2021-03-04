---
title: tipo de recurso permissionGrantPolicy
description: Especifica as condições em que o consentimento pode ser autorizado.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 89d6dccf4f9343fc27e2fae4ee7dff3bec89142c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444039"
---
# <a name="permissiongrantpolicy-resource-type"></a>tipo de recurso permissionGrantPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma política de concessão de permissão é usada para especificar as condições em que o consentimento pode ser concedido.

Uma política de concessão de permissão consiste em uma lista de conjuntos de condições **inclusos** e uma lista de conjuntos de condições **exclusos**. Para que um evento corresponda a uma política de concessão de permissão, ele deve corresponder a *pelo menos um* do conjunto de condições **incluso** e *nenhum* do conjuntos de condições **excluso**.

## <a name="methods"></a>Methods

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Política de concessão de permissões de lista](../api/permissiongrantpolicy-list.md) | conjunto [permissionGrantPolicy](permissiongrantpolicy.md) | Recupere uma lista de objetos permissionGrantPolicy. |
|[Cria política de concessão de permissões](../api/permissiongrantpolicy-post-permissiongrantpolicies.md)| [permissionGrantPolicy](permissiongrantpolicy.md) | Cria um novo objeto permissionGrantPolicy. |
|[Obter política de concessão de permissão](../api/permissiongrantpolicy-get.md) | [permissionGrantPolicy](permissiongrantpolicy.md) |Ler propriedades e relações do objeto permissionGrantPolicy.|
|[Política de concessão de permissões atualizada](../api/permissiongrantpolicy-update.md) | [permissionGrantPolicy](permissiongrantpolicy.md)  |Atualiza o objeto permissionGrantPolicy. |
|**Incluir conjuntos de condições**| | |
|[A lista inclui conjuntos de condições](../api/permissiongrantpolicy-list-includes.md) |conjunto de [permissionGrantConditionSet](permissiongrantconditionset.md)| Obtenha os conjuntos de condições *incluídos* nesta política de concessão de permissão.|
|[Adicionar conjuntos de condições de inclusão](../api/permissiongrantpolicy-post-includes.md) |[permissionGrantConditionSet](permissiongrantconditionset.md) | Adicione um conjunto de condições que foi *incluído* desta política de concessão de permissão. |
|[Remover conjuntos de condições de inclusão](../api/permissiongrantpolicy-delete-includes.md) | Nenhum | Remove um conjunto de condições que foi *excluído* desta política de concessão de permissão.|
|**Excluir conjuntos de condições**| | |
|[Listar conjuntos de condições de exclusão](../api/permissiongrantpolicy-list-excludes.md) |conjunto de [permissionGrantConditionSet](permissiongrantconditionset.md)| Obtenha os conjuntos de condições *excluídos* nesta política de concessão de permissão.|
|[Adicionar conjuntos de condições de exclusão](../api/permissiongrantpolicy-post-excludes.md) |[permissionGrantConditionSet](permissiongrantconditionset.md) | Adicione um conjunto de condições que foi *excluído* desta política de concessão de permissão. |
|[Remover conjuntos de condições de exclusão](../api/permissiongrantpolicy-delete-excludes.md) | Nenhum | Remove um conjunto de condições que foi *excluído* desta política de concessão de permissão.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo |Descrição|
|:---------------|:--------|:----------|
| id | String | O identificador exclusivo da política de concessão de permissão. O prefixo de **identificação**`microsoft-` está reservado para políticas de concessão de permissão interna e não pode ser usado em uma política de concessão de permissão personalizada. Somente letras, números, hifens (`-`) e sublinhados (`_`) são permitidos. Chave. Não anulável. Obrigatório durante a criação. Imutável. |
| displayName | String |O nome de exibição da política de concessão de permissão.|
| descrição |String| A descrição da política de concessão de permissão.|
| inclui | conjunto de [permissionGrantConditionSet](permissiongrantconditionset.md)| Os conjuntos de condições *incluídos* nesta política de concessão de permissão. Expandida automaticamente no `GET`.|
| exclui |conjunto de [permissionGrantConditionSet](permissiongrantconditionset.md)| Conjuntos de condições *excluídos* nesta política de concessão de permissão. Expandida automaticamente no `GET`.|

## <a name="relationships"></a>Relações

| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|inclui|conjunto de [permissionGrantConditionSet](permissiongrantconditionset.md)| Os conjuntos de condições *incluídos* nesta política de concessão de permissão. Essa navegação é expandida automaticamente no GET. |
|exclui|conjunto de [permissionGrantConditionSet](permissiongrantconditionset.md)| Conjuntos de condições *excluídos* nesta política de concessão de permissão. Essa navegação é expandida automaticamente no GET. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.permissionGrantPolicy"
}-->

```json
{
  "id": "string (identifier)",
  "displayName": "string",
  "description": "string",
  "includes": "collection(microsoft.graph.permissionGrantConditionSet)",
  "excludes": "collection(microsoft.graph.permissionGrantConditionSet)"
}
```
