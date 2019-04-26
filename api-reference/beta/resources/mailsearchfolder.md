---
title: tipo de recurso mailSearchFolder
description: Um mailSearchFolder é uma pasta virtual na caixa de correio do usuário que contém todos os itens de email correspondentes aos critérios de pesquisa especificados. mailSearchFolder herda de mailFolder.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 15f334f2910c962c367242965bd2104c8f3edb79
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342742"
---
# <a name="mailsearchfolder-resource-type"></a>tipo de recurso mailSearchFolder

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um mailSearchFolder é uma pasta virtual na caixa de correio do usuário que contém todos os itens de email correspondentes aos critérios de pesquisa especificados. mailSearchFolder herda de [mailFolder](mailfolder.md).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno  | Descrição |
|:---------------|:--------|:----------|
| [Criar uma pasta de pesquisa](../api/mailsearchfolder-post.md) | [mailSearchFolder](mailsearchfolder.md) | Crie uma pasta de pesquisa na caixa de correio do usuário. |
| [Listar pastas de pesquisa](../api/mailfolder-list-childfolders.md) | Coleção [mailFolder](mailfolder.md) | Listar todas as pastas na caixa de correio do usuário, incluindo pastas de pesquisa. |
| [Obter uma pasta de pesquisa](../api/mailfolder-get.md) | [mailSearchFolder](mailsearchfolder.md) | Obtém a pasta de pesquisa especificada. |
| [Atualizar uma pasta de pesquisa](../api/mailsearchfolder-update.md) | [mailSearchFolder](mailsearchfolder.md) | Atualiza a pasta de pesquisa especificada. |
| [Excluir uma pasta de pesquisa](../api/mailfolder-delete.md) | Nenhum | Excluir a pasta de pesquisa especificada. |
| [Listar todas as mensagens em uma pasta de pesquisa](../api/mailfolder-list-messages.md) | Coleção [message](message.md) | Listar todas as mensagens na pasta de pesquisa especificada. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| isSupported | Boolean | Indica se uma pasta de pesquisa é editável usando as APIs REST. |
| includeNestedFolders | Boolean | Indica como a hierarquia da pasta da caixa de correio deve ser percorrida. `true`significa que uma pesquisa profunda deve ser feita enquanto `false` uma pesquisa superficial deve ser realizada. |
| sourceFolderIDs | Coleção String | As pastas de caixa de correio que devem ser minadas. |
| filterQuery | String | A consulta OData para filtrar as mensagens. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailSearchFolder"
}-->

```json
{
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": ["string"],
  "filterQuery": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2018-01-23 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
