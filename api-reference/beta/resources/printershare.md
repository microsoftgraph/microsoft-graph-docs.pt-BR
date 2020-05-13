---
title: tipo de recurso printerShare
description: Representa uma impressora que pretende ser detectável por usuários e por aplicativos de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5acbcdc58b730404a39af1f3069b3433fac54ed3
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217344"
---
# <a name="printershare-resource-type"></a>tipo de recurso printerShare

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma impressora que pretende ser detectável por usuários e por aplicativos de impressão.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar](../api/print-list-shares.md) | coleção [printerShare](printershare.md) | Obtenha uma lista de compartilhamentos de impressora no locatário. |
| [Get](../api/printershare-get.md) | [printerShare](printershare.md) | Ler propriedades e relações de um objeto **printerShare** . |
| [Update](../api/printershare-update.md) | [printerShare](printershare.md) | Atualizar um objeto **printerShare** . |
| [Delete](../api/printershare-delete.md) | Nenhum | Descompartilhar uma impressora. |
| [Listar allowedUsers](../api/printershare-list-allowedusers.md) | coleção [printUserIdentity](printuseridentity.md) | Recupere uma lista de usuários que receberam acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado. |
| [Adicionar allowedUser](../api/printershare-post-allowedusers.md) | Nenhum | Conceda ao usuário especificado o acesso ao envio de trabalhos de impressão para o compartilhamento de impressora associado. |
| [Remover allowedUser](../api/printershare-delete-alloweduser.md) | Nenhum | Revoga o acesso ao compartilhamento de impressora do usuário especificado. |
| [Listar allowedGroups](../api/printershare-list-allowedgroups.md) | coleção [Multiidentity](printidentity.md) | Recupere uma lista de grupos aos quais foi concedido acesso para enviar trabalhos de impressão ao compartilhamento de impressora associado. |
| [Adicionar allowedGroup](../api/printershare-post-allowedgroups.md) | Nenhum | Conceda ao grupo especificado o acesso ao envio de trabalhos de impressão para o compartilhamento de impressora associado. |
| [Remover allowedGroup](../api/printershare-delete-allowedgroup.md) | Nenhum | Revoga o acesso ao compartilhamento de impressora do grupo especificado. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| O identificador do printerShare. Somente leitura.|
|displayName|Cadeia de caracteres|O nome do compartilhamento de impressora que os clientes de impressão devem exibir.|
|createdDateTime|DateTimeOffset|O DateTimeOffset quando o compartilhamento da impressora foi criado. Somente leitura.|
|fabricante|String|O fabricante relatado pela impressora associada a este compartilhamento de impressora. Somente leitura.|
|modelo|String|O nome do modelo relatado pela impressora associada a este compartilhamento de impressora. Somente leitura.|
|isAcceptingJobs|Boolean|Se a impressora associada a este compartilhamento de impressora está atualmente aceitando novos trabalhos de impressão.|
|padrões|[printerDefaults](printerdefaults.md)|As configurações de impressão padrão da impressora associadas a este compartilhamento de impressora.|
|capabilities|[printerCapabilities](printercapabilities.md)|Os recursos da impressora associada a este compartilhamento de impressora.|
|location|[printerLocation](printerlocation.md)|O local físico e/ou organizacional da impressora associado a este compartilhamento de impressora.|
|status|[printerStatus](printerstatus.md)|O status de processamento, incluindo qualquer erro, da impressora associada a este compartilhamento de impressora. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|impressora|[impressora](printer.md)|A impressora à qual esse compartilhamento de impressora está relacionado. |
|allowedUsers|coleção [printUserIdentity](printuseridentity.md)|Os usuários que têm acesso à impressão usando a impressora.|
|allowedGroups|[multiidentity](printidentity.md)|Os grupos cujos usuários têm acesso para imprimir usando a impressora.|
|serviços|coleção [printJob](printjob.md)| A lista de trabalhos que estão na fila para impressão pela impressora associada a este compartilhamento de impressora.|

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
