---
title: tipo de recurso printerShare
description: Representa uma impressora que pretende ser detectável por usuários e por aplicativos de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5f8b8ad8446d37c73ddfd2b55b8ca544f1f926cd
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49664072"
---
# <a name="printershare-resource-type"></a>tipo de recurso printerShare

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma impressora que pretende ser detectável por usuários e por aplicativos de impressão.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/print-list-shares.md) | coleção [printerShare](printershare.md) | Obtenha uma lista de compartilhamentos de impressora no locatário. |
| [Get](../api/printershare-get.md) | [printerShare](printershare.md) | Ler propriedades e relações de um objeto **printerShare** . |
| [Atualizar](../api/printershare-update.md) | [printerShare](printershare.md) | Atualizar um objeto **printerShare** . |
| [Delete](../api/printershare-delete.md) | Nenhum | Descompartilhar uma impressora. |
| [Listar trabalhos](../api/printershare-list-jobs.md) | coleção [printJob](printjob.md) | Obtenha uma lista de trabalhos de impressão que são enfileirados para processamento pelo printerShare. |
| [Criar trabalho](../api/printershare-post-jobs.md) | [Impressão](printjob.md) | Criar um novo trabalho de impressão para o printerShare. Para começar a imprimir o trabalho, use [Iniciar](../api/printjob-start.md). |
| [Listar allowedUsers](../api/printershare-list-allowedusers.md) | Coleção [user](user.md) | Recupere uma lista de usuários que receberam acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado. |
| [Adicionar allowedUser](../api/printershare-post-allowedusers.md) | Nenhum | Conceda ao usuário especificado o acesso ao envio de trabalhos de impressão para o compartilhamento de impressora associado. |
| [Remover allowedUser](../api/printershare-delete-alloweduser.md) | Nenhum | Revoga o acesso ao compartilhamento de impressora do usuário especificado. |
| [Listar allowedGroups](../api/printershare-list-allowedgroups.md) | Coleção [group](group.md) | Recupere uma lista de grupos aos quais foi concedido acesso para enviar trabalhos de impressão ao compartilhamento de impressora associado. |
| [Adicionar allowedGroup](../api/printershare-post-allowedgroups.md) | Nenhum | Conceda ao grupo especificado o acesso ao envio de trabalhos de impressão para o compartilhamento de impressora associado. |
| [Remover allowedGroup](../api/printershare-delete-allowedgroup.md) | Nenhum | Revoga o acesso ao compartilhamento de impressora do grupo especificado. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| O identificador do printerShare. Somente leitura.|
|displayName|String|O nome do compartilhamento de impressora que os clientes de impressão devem exibir.|
|createdDateTime|DateTimeOffset|O DateTimeOffset quando o compartilhamento da impressora foi criado. Somente leitura.|
|fabricante|String|O fabricante relatado pela impressora associada a este compartilhamento de impressora. Somente leitura.|
|modelo|String|O nome do modelo relatado pela impressora associada a este compartilhamento de impressora. Somente leitura.|
|isAcceptingJobs|Boolean|Se a impressora associada a este compartilhamento de impressora está atualmente aceitando novos trabalhos de impressão.|
|defaults|[printerDefaults](printerdefaults.md)|As configurações de impressão padrão da impressora associadas a este compartilhamento de impressora.|
|capabilities|[printerCapabilities](printercapabilities.md)|Os recursos da impressora associada a este compartilhamento de impressora.|
|localização|[printerLocation](printerlocation.md)|O local físico e/ou organizacional da impressora associado a este compartilhamento de impressora.|
|status|[printerStatus](printerstatus.md)|O status de processamento, incluindo qualquer erro, da impressora associada a este compartilhamento de impressora. Somente leitura.|
|allowAllUsers|Boolean|Se true, todos os usuários e grupos terão acesso a esse compartilhamento de impressora. Isso substitui as listas de permissões definidas pelas propriedades de navegação **allowedUsers** e **allowedGroups** .|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|impressora|[impressora](printer.md)|A impressora à qual esse compartilhamento de impressora está relacionado. |
|allowedUsers|Coleção [user](user.md)|Os usuários que têm acesso à impressão usando a impressora.|
|allowedGroups|[group](group.md)|Os grupos cujos usuários têm acesso para imprimir usando a impressora.|
|jobs|coleção [printJob](printjob.md)| A lista de trabalhos que estão na fila para impressão pela impressora associada a este compartilhamento de impressora.|

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


