---
title: Tipo de recurso groupLifecyclePolicy
description: Representa uma política de ciclo de vida para um Microsoft 365 grupo.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 3122c297564981e75516ea602e699d3ebe49fa50
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317221"
---
# <a name="grouplifecyclepolicy-resource-type"></a>Tipo de recurso groupLifecyclePolicy

Namespace: microsoft.graph

Representa uma política de ciclo de vida para um Microsoft 365 grupo. Uma política de ciclo de vida permite aos administradores definir um período de validade para os grupos. Por exemplo, após 180 dias o grupo expira. Quando um grupo alcança esse prazo, os proprietários devem renovar o grupo por um período definido pelo administrador. Depois de renovado, o período de validade é estendido de acordo com o número de dias definido na política. Por exemplo, a nova validade do grupo é de 180 dias após a renovação. Caso não seja renovado, ele expirará e será excluído. É possível renovar o grupo no prazo de 30 dias da data de exclusão.

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Obter groupLifecyclePolicy](../api/grouplifecyclepolicy-get.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md) |Leia as propriedades e os relacionamentos de um objeto groupLifecyclePolicy.|
|[Listar groupLifecyclePolicies](../api/grouplifecyclepolicy-list.md) | Coleção [groupLifecyclePolicy](grouplifecyclepolicy.md) | Listar todos os objetos groupLifecyclePolicies. |
|[Atualizar groupLifecyclePolicy](../api/grouplifecyclepolicy-update.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md) | Atualizar um objeto groupLifecyclePolicy. |
|[Excluir groupLifecyclePolicy](../api/grouplifecyclepolicy-delete.md) | Nenhum | Excluir um objeto groupLifecyclePolicy. |
|[Adicionar um grupo a um objeto groupLifecyclePolicy](../api/grouplifecyclepolicy-addgroup.md)|Nenhum| Adicionar um grupo a uma política de ciclo de vida |
|[Remover um grupo de um objeto groupLifecyclePolicy](../api/grouplifecyclepolicy-removegroup.md)|Nenhum| Remover um grupo de uma política de ciclo de vida. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|alternateNotificationEmails|Cadeia de caracteres| Lista de endereços de email para o envio de notificações para grupos sem proprietários. É possível definir vários endereços de email separando-os com ponto-e-vírgula. |
|groupLifetimeInDays|Int32| Número de dias antes que um grupo expire e precise ser renovado. Após renová-lo, o período de validade é estendido de acordo com o número de dias definido. |
|id|Cadeia de caracteres| Um identificador exclusivo de uma política. Somente leitura.|
|managedGroupTypes|Cadeia de caracteres| O tipo de grupo ao qual se aplica a política de expiração. Os valores possíveis são **All**, **Selected** ou **None**. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
}-->

```json
{
  "alternateNotificationEmails": "String",
  "groupLifetimeInDays": 180,
  "id": "Guid (identifier)",
  "managedGroupTypes": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

