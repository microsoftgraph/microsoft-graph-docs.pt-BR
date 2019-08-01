---
title: tipo de recurso mailSearchFolder
description: Um mailSearchFolder é uma pasta virtual na caixa de correio do usuário que contém todos os itens de email correspondentes aos critérios de pesquisa especificados. mailSearchFolder herda de mailFolder.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f646cc24b7f451dc2662342a87b9ecbdd0b6dbc2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036334"
---
# <a name="mailsearchfolder-resource-type"></a>tipo de recurso mailSearchFolder

Um **mailSearchFolder** é uma pasta virtual na caixa de correio do usuário que contém todos os itens de email correspondentes aos critérios de pesquisa especificados. **mailSearchFolder** herda de [mailFolder](mailfolder.md). Pastas de pesquisa podem ser criadas em qualquer pasta da caixa de correio do Exchange Online de um usuário. No entanto, para que uma pasta de pesquisa apareça no Outlook, no Outlook para a Web ou no Outlook Live, a pasta deve ser criada na pasta **WellKnownFolderName. SearchFolders** . 

## <a name="search-folder-lifecycle"></a>Ciclo de vida da pasta de pesquisa

Pastas de pesquisa criadas por seu aplicativo podem ser excluídas pelo Exchange Online por uma das seguintes razões:

1.  As pastas de pesquisa expiram após 45 dias sem uso. 
2.  Há limites no número de pastas de pesquisa que podem ser criadas por pasta de origem. Quando esse limite é violado, as pastas de pesquisa mais antigas são excluídas para se tornarem novas. 

Quando uma pasta de pesquisa é excluída, seu aplicativo deve criar um novo recurso de pasta de pesquisa e usar o mesmo.


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
| IsSupported | Booliano | Indica se uma pasta de pesquisa é editável usando as APIs REST. |
| includeNestedFolders | Booliano | Indica como a hierarquia da pasta da caixa de correio deve ser percorrida na pesquisa. `true`significa que uma pesquisa profunda deve ser feita para incluir pastas filhas na hierarquia de cada pasta explicitamente especificada no **sourceFolderIds**. `false`significa uma pesquisa superficial de apenas cada uma das pastas explicitamente especificadas no **sourceFolderIds**. |
| sourceFolderIds | Coleção de cadeias de caracteres | As pastas de caixa de correio que devem ser minadas. |
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
  "sourceFolderIds": ["string"],
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
