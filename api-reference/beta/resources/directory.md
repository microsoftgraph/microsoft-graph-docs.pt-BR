---
title: Tipo de recurso directory (itens excluídos)
description: . Itens excluídos permanecerão disponíveis para restauração por até 30 dias. Após 30 dias, esses itens serão excluídos permanentemente.
ms.openlocfilehash: 74b4d1ff94b567557fd90701b1c4bae479a8317e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040337"
---
# <a name="directory-resource-type-deleted-items"></a>Tipo de recurso directory (itens excluídos)

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um item excluído no diretório. Quando um item é excluído, ele é adicionado ao "contêiner" de itens excluídos. Itens excluídos permanecerão disponíveis para restauração por até 30 dias. Após 30 dias, esses itens serão excluídos permanentemente.

Atualmente, a funcionalidade de itens excluídos apenas tem suporte para [grupos](group.md) e [usuários](users.md) do Office 365.

## <a name="methods"></a>Métodos

| Método         | Tipo de retorno | Descrição |
|:---------------|:------------|:------------|
|[Obter item excluído](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | Obtém as propriedades de um item excluído. |
|[Restaurar item excluído](../api/directory-deleteditems-restore.md) |[directoryObject](directoryobject.md)| Restaura um item recentemente excluído. |
|[Listar itens excluídos](../api/directory-deleteditems-list.md) |Coleção [directoryObject](directoryobject.md)| Obtém uma lista de itens recentemente excluídos. |
|[Excluir permanentemente um item](../api/directory-deleteditems-delete.md) | Nenhum | Exclui permanentemente um item. |
|[Listar itens excluídos pertencentes a um usuário](../api/directory-deleteditems-user-owned.md) | Coleção [directoryObject](directoryobject.md) | Lista os itens de diretório pertencentes a um usuário. |

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres| Um identificador exclusivo para o objeto; por exemplo, 12345678-9abc-def0-1234-56789abcde. Chave. Não anulável. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|deleteditems|Coleção [directoryObject](directoryobject.md)| Itens recentemente excluídos. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
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
<!-- {
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->