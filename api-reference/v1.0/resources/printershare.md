---
title: Tipo de recurso printerShare
description: Representa uma impressora que se destina a ser descoberta por usuários e aplicativos de impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: ec674121a0d8785ee68b9939a10e42272924c5d1a2a1d6cd37b7a5a4c650cf26
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218447"
---
# <a name="printershare-resource-type"></a>Tipo de recurso printerShare

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Representa uma impressora que se destina a ser descoberta por usuários e aplicativos de impressão.

Herda de [printerBase](../resources/printerbase.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [List](../api/print-list-shares.md) | [Coleção printerShare](printershare.md) | Obter uma lista de compartilhamentos de impressora no locatário. |
| [Obter](../api/printershare-get.md) | [printerShare](printershare.md) | Ler propriedades e relações de um **objeto printerShare.** |
| [Atualizar](../api/printershare-update.md) | [printerShare](printershare.md) | Atualize um **objeto printerShare.** |
| [Delete](../api/printershare-delete.md) | None | Desaque o compartilhamento de uma impressora. |
| [Listar trabalhos](../api/printershare-list-jobs.md) | [Coleção printJob](printjob.md) | Obter uma lista de trabalhos de impressão que estão na fila para processamento pela printerShare. |
| [Criar trabalho](../api/printershare-post-jobs.md) | [printJob](printjob.md) | Crie um novo trabalho de impressão para a printerShare. Para começar a imprimir o trabalho, use [start](../api/printjob-start.md). |
| [Listar allowedUsers](../api/printershare-list-allowedusers.md) | Coleção [user](user.md) | Recupere uma lista de usuários que tiveram acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado. |
| [Adicionar allowedUser](../api/printershare-post-allowedusers.md) | None | Conceda ao usuário especificado acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado. |
| [Remover allowedUser](../api/printershare-delete-alloweduser.md) | None | Revogar o acesso de compartilhamento de impressora do usuário especificado. |
| [Listar allowedGroups](../api/printershare-list-allowedgroups.md) | Coleção [group](group.md) | Recupere uma lista de grupos que tiveram acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado. |
| [Adicionar allowedGroup](../api/printershare-post-allowedgroups.md) | None | Conceda ao grupo especificado acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado. |
| [Remover allowedGroup](../api/printershare-delete-allowedgroup.md) | None | Revogar o acesso de compartilhamento de impressora do grupo especificado. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres| O identificador printerShare. Herdado de [printerBase](../resources/printerbase.md). Somente leitura.|
|displayName|Cadeia de caracteres|O nome do compartilhamento de impressora que os clientes de impressão devem exibir. Herdado de [printerBase](../resources/printerbase.md).|
|createdDateTime|DateTimeOffset|DateTimeOffset quando o compartilhamento de impressora foi criado. Somente leitura.|
|fabricante|String|O fabricante relatado pela impressora associada a esse compartilhamento de impressora. Herdado de [printerBase](../resources/printerbase.md). Somente leitura.|
|modelo|String|O nome do modelo relatado pela impressora associada a esse compartilhamento de impressora. Herdado de [printerBase](../resources/printerbase.md). Somente leitura.|
|isAcceptingJobs|Booliano|Se a impressora associada a esse compartilhamento de impressoras está aceitando novos trabalhos de impressão no momento. Herdado de [printerBase](../resources/printerbase.md).|
|defaults|[printerDefaults](printerdefaults.md)|As configurações de impressão padrão da impressora associada a esse compartilhamento de impressora. Herdado de [printerBase](../resources/printerbase.md).|
|capabilities|[printerCapabilities](printercapabilities.md)|Os recursos da impressora associados a esse compartilhamento de impressora. Herdado de [printerBase](../resources/printerbase.md).|
|localização|[printerLocation](printerlocation.md)|O local físico e/ou organizacional da impressora associada a esse compartilhamento de impressora. Herdado de [printerBase](../resources/printerbase.md).|
|status|[printerStatus](printerstatus.md)|O status do processamento, incluindo quaisquer erros, da impressora associada a esse compartilhamento de impressora. Herdado de [printerBase](../resources/printerbase.md). Apenas leitura.|
|allowAllUsers|Booliano|Se for true, todos os usuários e grupos terão acesso a esse compartilhamento de impressora. Isso sobressalta as listas de permissão definidas pelas propriedades de navegação **allowedUsers** e **allowedGroups.**|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|impressora|[impressora](printer.md)|A impressora à que essa impressora está relacionada. |
|allowedUsers|Coleção [usuário](user.md)|Os usuários que têm acesso à impressão usando a impressora.|
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

