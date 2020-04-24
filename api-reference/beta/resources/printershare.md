---
title: tipo de recurso printerShare
description: Representa uma impressora que pretende ser detectável por usuários e por aplicativos de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 8aa9312bf8b7e8f9a2cec049b8275d4ce7a04012
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2020
ms.locfileid: "43806847"
---
# <a name="printershare-resource-type"></a>tipo de recurso printerShare

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma impressora que pretende ser detectável por usuários e por aplicativos de impressão.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/print-list-printershares.md) | coleção [printerShare](printershare.md) | Obtenha uma lista de compartilhamentos de impressora no locatário. |
| [Get](../api/printershare-get.md) | [printerShare](printershare.md) | Ler propriedades e relações de um objeto **printerShare** . |
| [Atualização](../api/printershare-update.md) | [printerShare](printershare.md) | Atualizar um objeto **printerShare** . |
| [Delete](../api/printershare-delete.md) | Nenhum | Descompartilhar uma impressora. |
| [Listar allowedUsers](../api/printershare-list-allowedusers.md) | coleção [UserIdentity](useridentity.md) | Recupere uma lista de usuários que receberam acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado. |
| [Adicionar allowedUser](../api/printershare-post-allowedusers.md) | Nenhum | Conceda ao usuário especificado o acesso ao envio de trabalhos de impressão para o compartilhamento de impressora associado. |
| [Remover allowedUser](../api/printershare-delete-alloweduser.md) | Nenhum | Revoga o acesso ao compartilhamento de impressora do usuário especificado. |
| [Listar allowedGroups](../api/printershare-list-allowedgroups.md) | coleção [Identity](identity.md) | Recupere uma lista de grupos aos quais foi concedido acesso para enviar trabalhos de impressão ao compartilhamento de impressora associado. |
| [Adicionar allowedGroup](../api/printershare-post-allowedgroups.md) | Nenhum | Conceda ao grupo especificado o acesso ao envio de trabalhos de impressão para o compartilhamento de impressora associado. |
| [Remover allowedGroup](../api/printershare-delete-allowedgroup.md) | Nenhum | Revoga o acesso ao compartilhamento de impressora do grupo especificado. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| O identificador do printerShare. Somente leitura.|
|name|String|O nome do compartilhamento de impressora que os clientes de impressão devem exibir.|
|createdDateTime|DateTimeOffset|O DateTimeOffset quando o compartilhamento da impressora foi criado. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|impressora|[impressora](printer.md)|A impressora à qual esse compartilhamento de impressora está relacionado. |
|allowedUsers|coleção [UserIdentity](useridentity.md)|Os usuários que têm acesso à impressão usando a impressora.|
|allowedGroups|[identity](identity.md)|Os grupos cujos usuários têm acesso para imprimir usando a impressora.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerShare",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerShare resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
