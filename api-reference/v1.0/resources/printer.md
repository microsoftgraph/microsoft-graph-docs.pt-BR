---
title: Tipo de recurso de impressora
description: Representa um dispositivo de impressora física que foi registrado com o serviço impressão universal. Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações de impressora, metadados de impressora e status de registro.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: e81614ba6c17955e8199e5c5aae6c643d93e9068
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232036"
---
# <a name="printer-resource-type"></a>Tipo de recurso de impressora

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Representa um dispositivo de impressora que foi registrado com o serviço impressão universal. Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações de impressora, metadados de impressora e status de registro.

Esse recurso permite:
* [Assinatura para alterar notificações](/graph/universal-print-webhook-notifications).

Herda de [printerBase](../resources/printerbase.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [Criar](../api/printer-create.md) | [printerCreateOperation](printerCreateOperation.md) | Criar (registrar) uma nova impressora com Impressão Universal. |
| [Get](../api/printer-get.md) | [impressora](printer.md) | Leia as propriedades e as relações do objeto printer. |
| [Atualização](../api/printer-update.md) | [impressora](printer.md) | Atualize o objeto printer. |
| [Delete](../api/printer-delete.md) | Nenhum | Desaconselhe a impressora física do serviço de Impressão Universal. |
| [restoreFactoryDefaults](../api/printer-restorefactorydefaults.md) | Nenhum | Restaure as configurações padrão de uma impressora para os valores especificados pelo fabricante. |
| [Listar trabalhos](../api/printer-list-jobs.md) | [Coleção printJob](printjob.md) | Obter uma lista de trabalhos de impressão que estão na fila para processamento pela impressora. |
| [Criar trabalho](../api/printer-post-jobs.md) | [printJob](printjob.md) | Crie um novo trabalho de impressão para a impressora. Para começar a imprimir o trabalho, use [start](../api/printjob-start.md). |
| [Listar conectores](../api/printer-list-connectors.md) | [Coleção printConnector](printconnector.md) | Obter uma lista de conectores que esta impressora está associada. |
| [Listar shares](../api/printer-list-shares.md) | [Coleção printerShare](printerShare.md) | Obter uma lista de printerShares que esta impressora está associada. Atualmente, apenas uma impressoraShare pode ser associada a uma impressora. |
| [List taskTriggers](../api/printer-list-tasktriggers.md) | Nenhum | Listar [printTaskTriggers](printtasktrigger.md) associados a essa impressora. |
| [Create taskTrigger](../api/printer-post-tasktriggers.md) | [printTaskTrigger](printtasktrigger.md) | Crie um [printTaskTrigger que](printtasktrigger.md) é executado quando ocorrem eventos de impressão. |
| [Delete taskTrigger](../api/printer-delete-tasktrigger.md) | Nenhum | [Exclua um printTaskTrigger](printtasktrigger.md) associado à impressora. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador do documento. Herdado de [printerBase](../resources/printerbase.md). Somente leitura.|
|displayName|String|O nome da impressora. Herdado de [printerBase](../resources/printerbase.md).|
|fabricante|String|O fabricante relatado pela impressora. Herdado de [printerBase](../resources/printerbase.md).|
|modelo|String|O nome do modelo relatado pela impressora. Herdado de [printerBase](../resources/printerbase.md).|
|registeredDateTime|DateTimeOffset|DateTimeOffset quando a impressora foi registrada. Somente leitura.|
|status|[printerStatus](printerstatus.md)|O status de processamento da impressora, incluindo quaisquer erros. Herdado de [printerBase](../resources/printerbase.md).|
|isShared|Booliano|True se a impressora for compartilhada; false caso contrário. Somente leitura.|
|hasPhysicalDevice|Booliano|True se a impressora tiver um dispositivo físico para impressão. Somente leitura.|
|isAcceptingJobs|Booliano|Se a impressora está aceitando novos trabalhos de impressão no momento. Herdado de [printerBase](../resources/printerbase.md).|
|localização|[printerLocation](printerlocation.md)|O local físico e/ou organizacional da impressora. Herdado de [printerBase](../resources/printerbase.md).|
|defaults|[printerDefaults](printerdefaults.md)|As configurações de impressão padrão da impressora. Herdado de [printerBase](../resources/printerbase.md).|
|capabilities|[printerCapabilities](printercapabilities.md)|Os recursos da impressora associados a esse compartilhamento de impressora. Herdado de [printerBase](../resources/printerbase.md).|
|lastSeenDateTime|DateTimeOffset|O dateTimeOffset mais recente quando uma impressora interagiu com a Impressão Universal. Somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|jobs|[Coleção printJob](printjob.md)| A lista de trabalhos que estão na fila para impressão pela impressora.  Herdado de [printerBase](../resources/printerbase.md).|
|shares|[Coleção printerShare](printershare.md)| A lista de printerShares que estão associadas à impressora. Atualmente, apenas uma impressoraShare pode ser associada à impressora. Somente leitura. Anulável.|
|conectores|[printConnector](printconnector.md)|Os conectores associados à impressora.|
|taskTriggers|[Coleção printTaskTrigger](printtasktrigger.md)|Uma lista de gatilhos de tarefas associados à impressora.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printer",
  "baseType": "microsoft.graph.printerBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printer",
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
  "registeredDateTime": "String (timestamp)",
  "isShared": "Boolean",
  "hasPhysicalDevice": "Boolean",
  "lastSeenDateTime": "String (timestamp)"
}
```

