---
title: tipo de recurso de impressora
description: Representa um dispositivo de impressora física que foi registrado com o serviço de impressão universal. Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações da impressora, metadados da impressora e status do registro.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: b86d3607decc8aca5b24b2be6f8344da87693fde
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703570"
---
# <a name="printer-resource-type"></a>tipo de recurso de impressora

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um dispositivo de impressora que foi registrado com o serviço de impressão universal. Os recursos de impressora podem ser usados para gerenciar trabalhos de impressão, configurações da impressora, metadados da impressora e status do registro.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar](../api/printer-create.md) | [printerCreateOperation](printerCreateOperation.md) | Criar (registrar) uma nova impressora com impressão universal. |
| [Get](../api/printer-get.md) | [impressora](printer.md) | Leia as propriedades e as relações do objeto Printer. |
| [Update](../api/printer-update.md) | [impressora](printer.md) | Atualize o objeto Printer. |
| [Delete](../api/printer-delete.md) | Nenhum | Cancelar o registro da impressora física do serviço de impressão universal. |
| [restoreFactoryDefaults](../api/printer-restorefactorydefaults.md) | Nenhum | Restaurar as configurações de padrões da impressora para os padrões de fábrica. |
| [Listar trabalhos](../api/printer-list-jobs.md) | coleção [printJob](printjob.md) | Obtenha uma lista de trabalhos de impressão que são enfileirados para processamento pela impressora. |
| [Criar trabalho](../api/printer-post-jobs.md) | [Impressão](printjob.md) | Crie um novo trabalho de impressão para a impressora. Para começar a imprimir o trabalho, use [Iniciar](../api/printjob-start.md). |
| [Listar conectores](../api/printer-list-connectors.md) | coleção [Multiconnector](printconnector.md) | Obter uma lista de conectores aos quais esta impressora está associada. |
| [List taskTriggers](../api/printer-list-tasktriggers.md) | Nenhum | Listar [printTaskTriggers](printtasktrigger.md) associados a essa impressora. |
| [Create taskTrigger](../api/printer-post-tasktriggers.md) | [printTaskTrigger](printtasktrigger.md) | Crie um [printTaskTrigger](printtasktrigger.md) que seja executado quando os eventos Print ocorrerem. |
| [Delete taskTrigger](../api/printer-delete-tasktrigger.md) | Nenhum | Excluir um [printTaskTrigger](printtasktrigger.md) que está associado à impressora. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|O identificador do documento. Somente leitura.|
|displayName|String|O nome da impressora.|
|fabricante|String|O fabricante relatado pela impressora. Somente leitura.|
|modelo|String|O nome do modelo relatado pela impressora. Somente leitura.|
|registeredDateTime|DateTimeOffset|O DateTimeOffset quando a impressora foi registrada. Somente leitura.|
|status|[printerStatus](printerstatus.md)|O status de processamento da impressora, incluindo erros. Somente leitura.|
|isShared|Booliano|True se a impressora é compartilhada; caso contrário, false. Somente leitura.|
|isAcceptingJobs|Boolean|Se a impressora está atualmente aceitando novos trabalhos de impressão.|
|location|[printerLocation](printerlocation.md)|O local físico e/ou organizacional da impressora.|
|defaults|[printerDefaults](printerdefaults.md)|As configurações de impressão padrão da impressora.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|jobs|coleção [printJob](printjob.md)| A lista de trabalhos que estão na fila para impressão pela impressora.|
|shares|coleção [printerShare](printershare.md)| A lista de printerShares que estão associados à impressora. Atualmente, apenas um printerShare pode ser associado à impressora. Somente leitura. Anulável.|
|conectores|[separador de Hiperligação](printconnector.md)|Os conectores associados à impressora.|
|taskTriggers|coleção [printTaskTrigger](printtasktrigger.md)|Uma lista de disparadores de tarefas que estão associados à impressora.|

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
  "name": "String",
  "manufacturer": "String",
  "model": "String",
  "isShared": true,
  "registeredDateTime": "String (timestamp)",
  "acceptingJobs": true,
  "registeredBy": {"@odata.type": "microsoft.graph.printUserIdentity"},
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "status": {"@odata.type": "microsoft.graph.printerStatus"},
  "defaults": {"@odata.type": "microsoft.graph.printerDefaults"}
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


