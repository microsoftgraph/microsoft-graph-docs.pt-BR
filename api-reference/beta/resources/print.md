---
title: tipo de recurso Print
description: Quando acompanhada por uma assinatura de impressão universal, o recurso de impressão permite o gerenciamento de impressoras e a descoberta de ServiceEndpoints que podem ser usados para gerenciar impressoras e trabalhos de impressão dentro do universal Print.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 309b7c8e62b94703bb00e21fb8c8ed2a2e917efe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985885"
---
# <a name="print-resource-type"></a>tipo de recurso Print

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Quando acompanhada por uma assinatura de impressão universal, o recurso de impressão permite o gerenciamento de impressoras e a descoberta de [ServiceEndpoints](printserviceendpoint.md) que podem ser usados para gerenciar impressoras e trabalhos de impressão dentro do universal Print.

## <a name="methods"></a>Methods
| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar conectores](../api/print-list-connectors.md) | coleção [Multiconnector](printconnector.md) | Obtenha uma lista de conectores de impressão. |
| [Lista de impressoras](../api/print-list-printers.md) | coleção de [impressoras](printer.md) | Obter uma lista de impressoras. |
| [Listar shares](../api/print-list-shares.md) | coleção [printerShare](printershare.md) | Obter uma lista de compartilhamentos de impressora. |
| [Listar serviços](../api/print-list-services.md) | coleção de [serviços de multiserviço](printservice.md) | Obtenha uma lista de serviços. |
| [Criar printerShare](../api/print-post-shares.md) | [printerShare](printershare.md) | Crie um novo compartilhamento de impressora postando na coleção de **compartilhamentos** . |
| [Criar impressora](../api/printer-create.md) | [printerCreateOperation](printerCreateOperation.md) | Criar (registrar) uma nova impressora com impressão universal. |
| [Atualizar configurações](../api/print-update-settings.md) |  [printSettings](printsettings.md) | Atualiza as configurações de todos os locatários para o serviço de impressão universal. |
| [Listar taskDefinitions](../api/print-list-taskdefinitions.md) | coleção [printTaskDefinition](printtaskdefinition.md) | Obter uma lista de todos os locatários de printTaskDefinitions criados dentro da impressão universal. |
| [Criar taskDefinition](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | Criar um novo printTaskDefinition. |
| [Atualizar taskDefinition](../api/print-update-taskdefinition.md) | [printTaskDefinition](printtaskdefinition.md) | Atualizar um printTaskDefinition. |
| [Excluir taskDefinition](../api/print-delete-taskdefinition.md) | Nenhum | Excluir um printTaskDefinition. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|settings|[printSettings](printsettings.md)|Configurações de todo o locatário para o serviço de impressão universal.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|serviço|coleção de [serviços de multiserviço](printservice.md)|A lista de pontos de extremidade do serviço de impressão Universal disponível.|
|impressoras|coleção de [impressoras](printer.md)|A lista de impressoras registradas no locatário.|
|shares|coleção [printerShare](printershare.md)|A lista de compartilhamentos de impressora registrados no locatário.|
|conectores|coleção [Multiconnector](printconnector.md)|A lista de conectores de impressão disponíveis.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.print",
  "keyProperty": "settings"
}-->

```json
{
  "settings": {"@odata.type": "microsoft.graph.printSettings"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "print resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [ 
    "Error: Resource print has documented navigation properties, but we thought it was a complex type!",
    "Resource print has documented navigation properties, but we thought it was a complex type!"
}-->


