---
title: Tipo de recurso mailSearchFolder
description: Um mailSearchFolder é uma pasta virtual na caixa de correio do usuário que contém todos os itens de email correspondentes aos critérios de pesquisa especificados. mailSearchFolder herda de mailFolder.
ms.localizationpriority: medium
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 077ba877c80987456278bec654b3622da2b1ecc3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036127"
---
# <a name="mailsearchfolder-resource-type"></a>Tipo de recurso mailSearchFolder

Namespace: microsoft.graph

Um **mailSearchFolder** é uma pasta virtual na caixa de correio do usuário que contém todos os itens de email correspondentes aos critérios de pesquisa especificados. **mailSearchFolder** herda de [mailFolder](mailfolder.md). As pastas de pesquisa podem ser criadas em qualquer pasta na caixa de correio Exchange Online usuário. No entanto, para que uma pasta de pesquisa apareça no Outlook, Outlook para a Web ou Outlook Live, a pasta deve ser criada na **pasta WellKnownFolderName.SearchFolders.** 

## <a name="search-folder-lifecycle"></a>Ciclo de vida da pasta de pesquisa

As pastas de pesquisa criadas pelo aplicativo podem ser excluídas por Exchange Online por um dos seguintes motivos:

1.  As pastas de pesquisa expiram após 45 dias sem uso. 
2.  Há limites no número de pastas de pesquisa que podem ser criadas por pasta de origem. Quando esse limite é violado, pastas de pesquisa mais antigas são excluídas para dar lugar a novas. 

Quando uma pasta de pesquisa é excluída, seu aplicativo deve criar um novo recurso de pasta de pesquisa e usar o mesmo.


## <a name="methods"></a>Métodos

| Método | Tipo de retorno  | Descrição |
|:---------------|:--------|:----------|
| [Criar uma pasta de pesquisa](../api/mailsearchfolder-post.md) | [mailSearchFolder](mailsearchfolder.md) | Crie uma pasta de pesquisa na caixa de correio desse usuário. |
| [Listar pastas de pesquisa](../api/mailfolder-list-childfolders.md) | Coleção [mailFolder](mailfolder.md) | Listar todas as pastas na caixa de correio desse usuário, incluindo pastas de pesquisa. |
| [Obter uma pasta de pesquisa](../api/mailfolder-get.md) | [mailSearchFolder](mailsearchfolder.md) | Obter a pasta de pesquisa especificada. |
| [Atualizar uma pasta de pesquisa](../api/mailsearchfolder-update.md) | [mailSearchFolder](mailsearchfolder.md) | Atualize a pasta de pesquisa especificada. |
| [Excluir uma pasta de pesquisa](../api/mailfolder-delete.md) | None | Exclua a pasta de pesquisa especificada. |
| [Listar todas as mensagens em uma pasta de pesquisa](../api/mailfolder-list-messages.md) | Coleção [message](message.md) | Lista todas as mensagens na pasta de pesquisa especificada. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| isSupported | Booliano | Indica se uma pasta de pesquisa é editável usando APIs REST. |
| includeNestedFolders | Boolean | Indica como a hierarquia de pastas de caixa de correio deve ser percorrido na pesquisa. `true` significa que uma pesquisa profunda deve ser feita para incluir pastas filho na hierarquia de cada pasta explicitamente especificada em **sourceFolderIds**. `false` significa uma pesquisa superficial de apenas cada uma das pastas explicitamente especificadas em **sourceFolderIds**. |
| sourceFolderIds | Coleção String | As pastas de caixa de correio que devem ser mineradas. |
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

