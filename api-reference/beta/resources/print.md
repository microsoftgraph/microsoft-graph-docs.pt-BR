---
title: tipo de recurso print
description: Quando acompanhado por uma assinatura de Impressão Universal, o recurso Imprimir permite o gerenciamento de impressoras e a descoberta de printServiceEndpoints que podem ser usados para gerenciar impressoras e trabalhos de impressão dentro da Impressão Universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 0604044824d153c9e6d39586c2ca58ee9ca893ea
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292249"
---
# <a name="print-resource-type"></a>tipo de recurso print

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Quando acompanhado por uma assinatura de Impressão Universal, o recurso Imprimir permite o gerenciamento de impressoras e a descoberta de [printServiceEndpoints](printserviceendpoint.md) que podem ser usados para gerenciar impressoras e trabalhos de impressão dentro da Impressão Universal.

## <a name="methods"></a>Métodos
| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar conectores](../api/print-list-connectors.md) | [Coleção printConnector](printconnector.md) | Obter uma lista de conectores de impressão. |
| [Lista de impressoras](../api/print-list-printers.md) | [coleção printer](printer.md) | Obter uma lista de impressoras. |
| [Listar shares](../api/print-list-shares.md) | [Coleção printerShare](printershare.md) | Obter uma lista de compartilhamentos de impressora. |
| [Listar serviços](../api/print-list-services.md) | [Coleção printService](printservice.md) | Obter uma lista de serviços. |
| [Criar printerShare](../api/print-post-shares.md) | [printerShare](printershare.md) | Crie um novo compartilhamento de impressora postando na coleção **shares.** |
| [Criar impressora](../api/printer-create.md) | [printerCreateOperation](printerCreateOperation.md) | Crie (registre) uma nova impressora com Impressão Universal. |
| [Atualizar configurações](../api/print-update-settings.md) |  [printSettings](printsettings.md) | Atualiza as configurações de todo o locatário para o serviço de Impressão Universal. |
| [Listar taskDefinitions](../api/print-list-taskdefinitions.md) | [Coleção printTaskDefinition](printtaskdefinition.md) | Obter uma lista de todos os locatários de printTaskDefinitions criadas na Impressão Universal. |
| [Criar taskDefinition](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | Crie uma nova printTaskDefinition. |
| [Atualizar taskDefinition](../api/print-update-taskdefinition.md) | [printTaskDefinition](printtaskdefinition.md) | Atualize uma printTaskDefinition. |
| [Excluir taskDefinition](../api/print-delete-taskdefinition.md) | Nenhum | Exclua uma printTaskDefinition. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|settings|[printSettings](printsettings.md)|Configurações para todo o locatário para o serviço de Impressão Universal.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|serviços|[Coleção printService](printservice.md)|A lista de pontos de extremidade de serviço de Impressão Universal disponíveis.|
|impressoras|[coleção printer](printer.md)|A lista de impressoras registradas no locatário.|
|shares|[Coleção printerShare](printershare.md)|A lista de compartilhamentos de impressora registrados no locatário.|
|conectores|[Coleção printConnector](printconnector.md)|A lista de conectores de impressão disponíveis.|

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
  ]
}-->


