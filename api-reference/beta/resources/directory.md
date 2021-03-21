---
title: Tipo de recurso directory (itens excluídos)
description: . Itens excluídos permanecerão disponíveis para restauração por até 30 dias. Após 30 dias, esses itens serão excluídos permanentemente.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4eb1cbdcbf0a1256c2bf2bf0cec35479b8bbc2cc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962620"
---
# <a name="directory-resource-type-deleted-items"></a>Tipo de recurso directory (itens excluídos)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um item excluído no diretório. Quando um item é excluído, ele é adicionado ao "contêiner" de itens excluídos. Itens excluídos permanecerão disponíveis para restauração por até 30 dias. Após 30 dias, esses itens serão excluídos permanentemente.

Atualmente, a funcionalidade de itens excluídos só tem suporte para os recursos [de](application.md)aplicativo, [grupo](group.md) [e](user.md) usuário.

## <a name="methods"></a>Métodos

| Método         | Tipo de retorno | Descrição |
|:---------------|:------------|:------------|
|[Obter item excluído](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | Obtém as propriedades de um item excluído. |
|[Restaurar item excluído](../api/directory-deleteditems-restore.md) |[directoryObject](directoryobject.md)| Restaura um item recentemente excluído. |
|[Listar itens excluídos](../api/directory-deleteditems-list.md) |Coleção [directoryObject](directoryobject.md)| Obtém uma lista de itens recentemente excluídos. |
|[Excluir permanentemente um item](../api/directory-deleteditems-delete.md) | Nenhum | Exclui permanentemente um item. |
|[Listar itens excluídos pertencentes a um usuário](../api/directory-deleteditems-user-owned.md) | Coleção [directoryObject](directoryobject.md) | Lista itens de diretório pertencentes a um usuário. |
|[Listar featureRolloutPolicies](../api/list-featurerolloutpolicies.md) | [Coleção featureRolloutPolicy](featurerolloutpolicy.md) | Recupere uma lista de objetos featureRolloutPolicy. |
|[Criar featureRolloutPolicy](../api/post-featurerolloutpolicies.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Crie um novo objeto featureRolloutPolicy. |
| [Obter featureRolloutPolicy](../api/featurerolloutpolicy-get.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Recupere as propriedades e as relações do objeto featurerolloutpolicy. |
| [Atualizar featureRolloutPolicy](../api/featurerolloutpolicy-update.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Atualize as propriedades do objeto featurerolloutpolicy. |
| [Excluir featureRolloutPolicy](../api/featurerolloutpolicy-delete.md) | Nenhum | Exclua um objeto featureRolloutPolicy. |

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres| Um identificador exclusivo para o objeto; por exemplo, 12345678-9abc-def0-1234-56789abcde. Chave. Não anulável. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|deleteditems|Coleção [directoryObject](directoryobject.md)| Itens recentemente excluídos. Somente leitura. Anulável.|
|featureRolloutPolicies|[Coleção featureRolloutPolicy](featurerolloutpolicy.md)| Anulável.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


