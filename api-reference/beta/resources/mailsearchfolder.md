---
title: tipo de recurso de mailSearchFolder
description: Um mailSearchFolder é uma pasta virtual na caixa de correio do usuário que contém todos os itens de email que correspondam a critérios de pesquisa especificado. mailSearchFolder herda de mailFolder.
localization_priority: Normal
ms.openlocfilehash: 62d4d8569977c99690e317a39a43bbc9d9dca3f1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870389"
---
# <a name="mailsearchfolder-resource-type"></a>tipo de recurso de mailSearchFolder

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Um mailSearchFolder é uma pasta virtual na caixa de correio do usuário que contém todos os itens de email que correspondam a critérios de pesquisa especificado. mailSearchFolder herda de [mailFolder](mailfolder.md).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno  | Descrição |
|:---------------|:--------|:----------|
| [Crie uma pasta de pesquisa](../api/mailsearchfolder-post.md) | [mailSearchFolder](mailsearchfolder.md) | Crie uma pasta de pesquisa na caixa de correio desse usuário. |
| [Lista as pastas de pesquisa](../api/mailfolder-list-childfolders.md) | Coleção [mailFolder](mailfolder.md) | Liste todas as pastas na caixa de correio do usuário, incluindo as pastas de pesquisa. |
| [Obtenha uma pasta de pesquisa](../api/mailfolder-get.md) | [mailSearchFolder](mailsearchfolder.md) | Obtenha a pasta de pesquisa especificado. |
| [Atualizar uma pasta de pesquisa](../api/mailsearchfolder-update.md) | [mailSearchFolder](mailsearchfolder.md) | Atualize a pasta de pesquisa especificado. |
| [Excluir uma pasta de pesquisa](../api/mailfolder-delete.md) | Nenhum | Exclua a pasta de pesquisa especificado. |
| [Listar todas as mensagens em uma pasta de pesquisa](../api/mailfolder-list-messages.md) | Coleção [message](message.md) | Liste todas as mensagens na pasta de pesquisa especificado. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| isSupported | Booliano | Indica se uma pasta de pesquisa é editável usando APIs REST. |
| includeNestedFolders | Booliano | Indica como a hierarquia de pastas de caixa de correio deve ser percorrida. `true`significa que uma profundidade de pesquisa deve ser feito ao `false` significa rasos de pesquisa devem ser feito em vez disso. |
| sourceFolderIDs | String collection | As pastas de caixa de correio que devem ser extraídas. |
| filterQuery | Cadeia de caracteres | A consulta OData para filtrar as mensagens. |

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
<!-- {
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
