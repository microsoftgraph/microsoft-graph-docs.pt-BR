---
title: tipo de recurso printer
description: Representa um dispositivo de impressora física que foi registrado com o serviço de Impressão Universal. Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações de impressora, metadados de impressora e status de registro.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: fab3e933608143846555c556a215025e39666257
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934867"
---
# <a name="printer-resource-type"></a>tipo de recurso printer

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um dispositivo de impressora que foi registrado com o serviço de Impressão Universal. Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações de impressora, metadados de impressora e status de registro.

Esse recurso permite:
* [Assinatura para alterar notificações](/graph/universal-print-webhook-notifications).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar](../api/printer-create.md) | [printerCreateOperation](printerCreateOperation.md) | Crie (registre) uma nova impressora com Impressão Universal. |
| [Get](../api/printer-get.md) | [impressora](printer.md) | Leia as propriedades e os relacionamentos do objeto printer. |
| [Update](../api/printer-update.md) | [impressora](printer.md) | Atualize o objeto printer. |
| [Delete](../api/printer-delete.md) | Nenhum | Unregister the physical printer from the Universal Print service. |
| [restoreFactoryDefaults](../api/printer-restorefactorydefaults.md) | Nenhum | Restaure as configurações padrão de uma impressora para os valores especificados pelo fabricante. |
| [Listar trabalhos](../api/printer-list-jobs.md) | [Coleção printJob](printjob.md) | Obter uma lista de trabalhos de impressão que estão na fila para processamento pela impressora. |
| [Criar trabalho](../api/printer-post-jobs.md) | [printJob](printjob.md) | Crie um novo trabalho de impressão para a impressora. Para começar a imprimir o trabalho, use [start](../api/printjob-start.md). |
| [Listar conectores](../api/printer-list-connectors.md) | [Coleção printConnector](printconnector.md) | Obter uma lista de conectores aos que esta impressora está associada. |
| [List taskTriggers](../api/printer-list-tasktriggers.md) | Nenhum | Listar [printTaskTriggers](printtasktrigger.md) associados a essa impressora. |
| [Create taskTrigger](../api/printer-post-tasktriggers.md) | [printTaskTrigger](printtasktrigger.md) | Crie um [printTaskTrigger que](printtasktrigger.md) seja executado quando ocorrerem eventos de impressão. |
| [Delete taskTrigger](../api/printer-delete-tasktrigger.md) | Nenhum | [Exclua um printTaskTrigger](printtasktrigger.md) associado à impressora. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|O identificador do documento. Somente leitura.|
|displayName|Cadeia de caracteres|O nome da impressora.|
|fabricante|String|O fabricante relatado pela impressora.|
|modelo|String|O nome do modelo relatado pela impressora.|
|registeredDateTime|DateTimeOffset|DateTimeOffset quando a impressora foi registrada. Somente leitura.|
|status|[printerStatus](printerstatus.md)|O status de processamento da impressora, incluindo quaisquer erros.|
|isShared|Booliano|True se a impressora for compartilhada; caso contrário, false. Somente leitura.|
|hasPhysicalDevice|Booliano|True se a impressora tiver um dispositivo físico para impressão. Somente leitura.|
|isAcceptingJobs|Booliano|Se a impressora está aceitando novos trabalhos de impressão no momento.|
|location|[printerLocation](printerlocation.md)|O local físico e/ou organizacional da impressora.|
|defaults|[printerDefaults](printerdefaults.md)|As configurações de impressão padrão da impressora.|
|capabilities|[printerCapabilities](printercapabilities.md)|Os recursos da impressora associada a esse compartilhamento de impressora.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|jobs|[Coleção printJob](printjob.md)| A lista de trabalhos que estão na fila para impressão pela impressora.|
|shares|[Coleção printerShare](printershare.md)| A lista de printerShares que estão associadas à impressora. Atualmente, apenas uma printerShare pode ser associada à impressora. Somente leitura. Anulável.|
|conectores|[printConnector](printconnector.md)|Os conectores associados à impressora.|
|taskTriggers|[Coleção printTaskTrigger](printtasktrigger.md)|Uma lista de gatilhos de tarefa que estão associados à impressora.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printer",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "isShared": true,
  "registeredDateTime": "String (timestamp)",
  "isAcceptingJobs": true,
  "hasPhysicalDevice": true,
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
  "description": "printer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


