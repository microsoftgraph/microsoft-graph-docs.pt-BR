---
title: Tipo de recurso printerShare
description: Representa uma impressora que se destina a ser descoberta por usuários e aplicativos de impressão.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 52d3bc8adedd8f05c4cc4493df533d074ce19f58
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944939"
---
# <a name="printershare-resource-type"></a>Tipo de recurso printerShare

Namespace: microsoft.graph

Representa uma impressora que se destina a ser descoberta por usuários e aplicativos de impressão.

Herda de [printerBase](../resources/printerbase.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [List](../api/print-list-shares.md) | [Coleção printerShare](printershare.md) | Obter uma lista de compartilhamentos de impressora no locatário. |
| [Get](../api/printershare-get.md) | [printerShare](printershare.md) | Ler propriedades e relações de um **objeto printerShare.** |
| [Atualizar](../api/printershare-update.md) | [printerShare](printershare.md) | Atualize um **objeto printerShare.** |
| [Delete](../api/printershare-delete.md) | Nenhum | Desaque o compartilhamento de uma impressora. |
| [Listar trabalhos](../api/printershare-list-jobs.md) | [Coleção printJob](printjob.md) | Obter uma lista de trabalhos de impressão que estão na fila para processamento pela printerShare. |
| [Criar trabalho](../api/printershare-post-jobs.md) | [printJob](printjob.md) | Crie um novo trabalho de impressão para a printerShare. Para começar a imprimir o trabalho, use [start](../api/printjob-start.md). |
| [Listar allowedUsers](../api/printershare-list-allowedusers.md) | Coleção [user](user.md) | Recupere uma lista de usuários que tiveram acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado. |
| [Adicionar allowedUser](../api/printershare-post-allowedusers.md) | Nenhum(a) | Conceda ao usuário especificado acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado. |
| [Remover allowedUser](../api/printershare-delete-alloweduser.md) | Nenhum(a) | Revogar o acesso de compartilhamento de impressora do usuário especificado. |
| [Listar allowedGroups](../api/printershare-list-allowedgroups.md) | Coleção [group](group.md) | Recupere uma lista de grupos que tiveram acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado. |
| [Adicionar allowedGroup](../api/printershare-post-allowedgroups.md) | Nenhum | Conceda ao grupo especificado acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado. |
| [Remover allowedGroup](../api/printershare-delete-allowedgroup.md) | Nenhum(a) | Revogar o acesso de compartilhamento de impressora do grupo especificado. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres| O identificador printerShare. Herdado de [printerBase](../resources/printerbase.md). Somente leitura.|
|displayName|Cadeia de caracteres|O nome do compartilhamento de impressora que os clientes de impressão devem exibir. Herdado de [printerBase](../resources/printerbase.md).|
|createdDateTime|DateTimeOffset|DateTimeOffset quando o compartilhamento de impressora foi criado. Somente leitura.|
|fabricante|String|O fabricante relatado pela impressora associada a esse compartilhamento de impressora. Herdado de [printerBase](../resources/printerbase.md). Somente leitura.|
|modelo|String|O nome do modelo relatado pela impressora associada a esse compartilhamento de impressora. Herdado de [printerBase](../resources/printerbase.md). Somente leitura.|
|isAcceptingJobs|Boolean|Se a impressora associada a esse compartilhamento de impressoras está aceitando novos trabalhos de impressão no momento. Herdado de [printerBase](../resources/printerbase.md).|
|defaults|[printerDefaults](printerdefaults.md)|As configurações de impressão padrão da impressora associada a esse compartilhamento de impressora. Herdado de [printerBase](../resources/printerbase.md).|
|capabilities|[printerCapabilities](printercapabilities.md)|Os recursos da impressora associados a esse compartilhamento de impressora. Herdado de [printerBase](../resources/printerbase.md).|
|localização|[printerLocation](printerlocation.md)|O local físico e/ou organizacional da impressora associada a esse compartilhamento de impressora. Herdado de [printerBase](../resources/printerbase.md).|
|status|[printerStatus](printerstatus.md)|O status do processamento, incluindo quaisquer erros, da impressora associada a esse compartilhamento de impressora. Herdado de [printerBase](../resources/printerbase.md). Somente leitura.|
|allowAllUsers|Boolean|Se for true, todos os usuários e grupos terão acesso a esse compartilhamento de impressora. Isso sobressalta as listas de permissão definidas pelas propriedades de navegação **allowedUsers** e **allowedGroups.**|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|impressora|[impressora](printer.md)|A impressora à que essa impressora está relacionada. |
|allowedUsers|Coleção [user](user.md)|Os usuários que têm acesso à impressão usando a impressora.|
|allowedGroups|[group](group.md)|Os grupos cujos usuários têm acesso para imprimir usando a impressora.|
|jobs|[Coleção printJob](printjob.md)| A lista de trabalhos que estão na fila para impressão pela impressora associada a esse compartilhamento de impressora.|
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printerShare",
  "baseType": "microsoft.graph.printerBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerShare",
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "isAcceptingJobs": "Boolean",
  "defaults": {
    "@odata.type": "microsoft.graph.printerDefaults"
  },
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "capabilities": {
    "@odata.type": "microsoft.graph.printerCapabilities"
  },
  "status": {
    "@odata.type": "microsoft.graph.printerStatus"
  },
  "allowAllUsers": "Boolean",
  "createdDateTime": "String (timestamp)"
}
```

