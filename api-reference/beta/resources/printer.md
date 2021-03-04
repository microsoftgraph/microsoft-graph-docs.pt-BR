---
title: Tipo de recurso de impressora
description: Representa um dispositivo de impressora física que foi registrado com o serviço impressão universal. Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações de impressora, metadados de impressora e status de registro.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 9adb08cd553857cbc7f7f9ebb257773b8775fa3f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442877"
---
# <a name="printer-resource-type"></a>Tipo de recurso de impressora

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um dispositivo de impressora que foi registrado com o serviço impressão universal. Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações de impressora, metadados de impressora e status de registro.

Esse recurso permite:
* [Assinatura para alterar notificações](/graph/universal-print-webhook-notifications).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar](../api/printer-create.md) | [printerCreateOperation](printerCreateOperation.md) | Criar (registrar) uma nova impressora com Impressão Universal. |
| [Get](../api/printer-get.md) | [impressora](printer.md) | Leia as propriedades e as relações do objeto printer. |
| [Atualização](../api/printer-update.md) | [impressora](printer.md) | Atualize o objeto printer. |
| [Delete](../api/printer-delete.md) | Nenhum(a) | Desaconselhe a impressora física do serviço de Impressão Universal. |
| [restoreFactoryDefaults](../api/printer-restorefactorydefaults.md) | Nenhum(a) | Restaure as configurações padrão de uma impressora para os valores especificados pelo fabricante. |
| [Listar trabalhos](../api/printer-list-jobs.md) | [Coleção printJob](printjob.md) | Obter uma lista de trabalhos de impressão que estão na fila para processamento pela impressora. |
| [Criar trabalho](../api/printer-post-jobs.md) | [printJob](printjob.md) | Crie um novo trabalho de impressão para a impressora. Para começar a imprimir o trabalho, use [start](../api/printjob-start.md). |
| [Listar conectores](../api/printer-list-connectors.md) | [Coleção printConnector](printconnector.md) | Obter uma lista de conectores que esta impressora está associada. |
| [List taskTriggers](../api/printer-list-tasktriggers.md) | Nenhum(a) | Listar [printTaskTriggers](printtasktrigger.md) associados a essa impressora. |
| [Create taskTrigger](../api/printer-post-tasktriggers.md) | [printTaskTrigger](printtasktrigger.md) | Crie um [printTaskTrigger que](printtasktrigger.md) é executado quando ocorrem eventos de impressão. |
| [Delete taskTrigger](../api/printer-delete-tasktrigger.md) | Nenhum(a) | [Exclua um printTaskTrigger](printtasktrigger.md) associado à impressora. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|O identificador do documento. Somente leitura.|
|displayName|String|O nome da impressora.|
|fabricante|String|O fabricante relatado pela impressora.|
|modelo|String|O nome do modelo relatado pela impressora.|
|registeredDateTime|DateTimeOffset|DateTimeOffset quando a impressora foi registrada. Somente leitura.|
|status|[printerStatus](printerstatus.md)|O status de processamento da impressora, incluindo quaisquer erros.|
|isShared|Booliano|True se a impressora for compartilhada; false caso contrário. Somente leitura.|
|hasPhysicalDevice|Booliano|True se a impressora tiver um dispositivo físico para impressão. Somente leitura.|
|isAcceptingJobs|Booliano|Se a impressora está aceitando novos trabalhos de impressão no momento.|
|localização|[printerLocation](printerlocation.md)|O local físico e/ou organizacional da impressora.|
|defaults|[printerDefaults](printerdefaults.md)|As configurações de impressão padrão da impressora.|
|capabilities|[printerCapabilities](printercapabilities.md)|Os recursos da impressora associados a esse compartilhamento de impressora.|
|lastSeenDateTime|DateTimeOffset|O dateTimeOffset mais recente quando uma impressora interagiu com a Impressão Universal. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|jobs|[Coleção printJob](printjob.md)| A lista de trabalhos que estão na fila para impressão pela impressora.|
|shares|[Coleção printerShare](printershare.md)| A lista de printerShares que estão associadas à impressora. Atualmente, apenas uma impressoraShare pode ser associada à impressora. Somente leitura. Anulável.|
|conectores|[printConnector](printconnector.md)|Os conectores associados à impressora.|
|taskTriggers|[Coleção printTaskTrigger](printtasktrigger.md)|Uma lista de gatilhos de tarefas associados à impressora.|

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
  "capabilities": {"@odata.type": "microsoft.graph.printerCapabilities"},
  "lastSeenDateTime": "String (timestamp)"
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


