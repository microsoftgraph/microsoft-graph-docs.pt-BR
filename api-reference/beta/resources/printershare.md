---
title: Tipo de recurso printerShare
description: Representa uma impressora que se destina a ser detectável por usuários e aplicativos de impressão.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: ab0dbf8ff2e7a8e64f51cf72afec5415bec265e6
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176685"
---
# <a name="printershare-resource-type"></a>Tipo de recurso printerShare

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma impressora que se destina a ser detectável por usuários e aplicativos de impressão.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/print-list-shares.md) | [Coleção printerShare](printershare.md) | Obtenha uma lista de compartilhamentos de impressora no locatário. |
| [Get](../api/printershare-get.md) | [printerShare](printershare.md) | Ler propriedades e relações de um **objeto printerShare** . |
| [Atualizar](../api/printershare-update.md) | [printerShare](printershare.md) | Atualize **um objeto printerShare** . |
| [Excluir](../api/printershare-delete.md) | Nenhum | Descompartilhar uma impressora. |
| [Listar trabalhos](../api/printershare-list-jobs.md) | [Coleção printJob](printjob.md) | Obtenha uma lista de trabalhos de impressão que estão na fila para processamento pela printerShare. |
| [Criar trabalho](../api/printershare-post-jobs.md) | [printJob](printjob.md) | Crie um novo trabalho de impressão para a printerShare. Para começar a imprimir o trabalho, use [start](../api/printjob-start.md). |
| [Listar allowedUsers](../api/printershare-list-allowedusers.md) | Coleção [user](user.md) | Recupere uma lista de usuários aos quais foi concedido acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado. |
| [Adicionar allowedUser](../api/printershare-post-allowedusers.md) | Nenhum | Conceda ao usuário especificado acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado. |
| [Remover allowedUser](../api/printershare-delete-alloweduser.md) | Nenhum | Revogar o acesso de compartilhamento de impressora do usuário especificado. |
| [Listar allowedGroups](../api/printershare-list-allowedgroups.md) | Coleção [group](group.md) | Recupere uma lista de grupos que recebeu acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado. |
| [Adicionar allowedGroup](../api/printershare-post-allowedgroups.md) | Nenhum | Conceda ao grupo especificado acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado. |
| [Remover allowedGroup](../api/printershare-delete-allowedgroup.md) | Nenhum | Revogar o acesso de compartilhamento de impressora do grupo especificado. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres| O identificador da printerShare. Somente leitura.|
|displayName|String|O nome do compartilhamento de impressora que os clientes de impressão devem exibir.|
|createdDateTime|DateTimeOffset|O DateTimeOffset quando o compartilhamento de impressora foi criado. Somente leitura.|
|fabricante|String|O fabricante relatado pela impressora associada a este compartilhamento de impressora. Somente leitura.|
|modelo|String|O nome do modelo relatado pela impressora associada a este compartilhamento de impressora. Somente leitura.|
|isAcceptingJobs|Booliano|Se a impressora associada a este compartilhamento de impressora está aceitando novos trabalhos de impressão no momento.|
|defaults|[printerDefaults](printerdefaults.md)|As configurações de impressão padrão da impressora associada a este compartilhamento de impressora.|
|capabilities|[printerCapabilities](printercapabilities.md)|Os recursos da impressora associada a este compartilhamento de impressora.|
|localização|[printerLocation](printerlocation.md)|O local físico e/ou organizacional da impressora associada a este compartilhamento de impressora.|
|status|[printerStatus](printerstatus.md)|O status de processamento, incluindo quaisquer erros, da impressora associada a este compartilhamento de impressora. Somente leitura.|
|allowAllUsers|Booliano|Se for true, todos os usuários e grupos receberão acesso a esse compartilhamento de impressora. Isso substitui as listas de permissão definidas pelas propriedades **de navegação allowedUsers** e **allowedGroups** .|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|Impressora|[impressora](printer.md)|A impressora à qual este compartilhamento de impressora está relacionado. |
|allowedUsers|Coleção [user](user.md)|Os usuários que têm acesso para imprimir usando a impressora.|
|allowedGroups|[group](group.md)|Os grupos cujos usuários têm acesso para imprimir usando a impressora.|
|jobs|[Coleção printJob](printjob.md)| A lista de trabalhos que estão na fila para impressão pela impressora associada a este compartilhamento de impressora.|

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
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "createdDateTime": "String (timestamp)",
  "isAcceptingJobs": true,
  "allowAllUsers": false,
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "status": {"@odata.type": "microsoft.graph.printerStatus"},
  "defaults": {"@odata.type": "microsoft.graph.printerDefaults"},
  "capabilities": {"@odata.type": "microsoft.graph.printerCapabilities"}
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


