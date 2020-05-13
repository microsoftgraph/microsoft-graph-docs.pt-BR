---
title: tipo de recurso Print
description: Quando acompanhada por uma assinatura de impressão universal, o recurso de impressão permite o gerenciamento de impressoras e a descoberta de ServiceEndpoints que podem ser usados para gerenciar impressoras e trabalhos de impressão dentro do universal Print.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: b0af3f7443b77920804f5868fe9ecc3f8b4cec41
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217084"
---
# <a name="print-resource-type"></a>tipo de recurso Print

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Quando acompanhada por uma assinatura de impressão universal, o recurso de impressão permite o gerenciamento de impressoras e a descoberta de [ServiceEndpoints](printserviceendpoint.md) que podem ser usados para gerenciar impressoras e trabalhos de impressão dentro do universal Print.

## <a name="methods"></a>Methods
| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Conectores de lista](../api/print-list-connectors.md) | coleção [Multiconnector](printconnector.md) | Obtenha uma lista de conectores de impressão. |
| [Listar impressoras](../api/print-list-printers.md) | coleção de [impressoras](printer.md) | Obter uma lista de impressoras. |
| [Lista de compartilhamentos](../api/print-list-shares.md) | coleção [printerShare](printershare.md) | Obter uma lista de compartilhamentos de impressora. |
| [Listar serviços](../api/print-list-services.md) | coleção de [serviços de multiserviço](printservice.md) | Obtenha uma lista de serviços. |
| [Criar printerShare](../api/print-post-shares.md) | [printerShare](printershare.md) | Crie um novo compartilhamento de impressora postando na coleção de **compartilhamentos** . |
| [Atualizar configurações](../api/print-update-settings.md) |  [printSettings](printsettings.md) | Atualiza as configurações de todos os locatários para o serviço de impressão universal. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|configurações|[printSettings](printsettings.md)|Configurações de todo o locatário para o serviço de impressão universal.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|serviço|coleção de [serviços de multiserviço](printservice.md)|A lista de pontos de extremidade do serviço de impressão Universal disponível.|
|impressoras|coleção de [impressoras](printer.md)|A lista de impressoras registradas no locatário.|
|shares|coleção [printerShare](printershare.md)|A lista de compartilhamentos de impressora registrados no locatário.|

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