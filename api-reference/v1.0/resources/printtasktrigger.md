---
title: Tipo de recurso printTaskTrigger
description: Determina as condições em que um novo printTask será executado com base na printTaskDefinition associada.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: ca4c5081521c2cbfd6e5ac4185548507f98e577ed2a590ded43d5788dde6cd9f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218419"
---
# <a name="printtasktrigger-resource-type"></a>Tipo de recurso printTaskTrigger

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Determina a condição na qual um [novo printTask](printtask.md) será acionado com base na [impressão associadaTaskDefinition](printtaskdefinition.md).

Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [List](../api/printer-list-tasktriggers.md) | [Coleção printTaskTrigger](printtasktrigger.md) | Obter uma lista de printTaskTriggers associados a uma impressora [específica.](printer.md) |
| [Obter](../api/printtasktrigger-get.md) | [printTaskTrigger](printtasktrigger.md) | Obter o printTaskTrigger associado a um [printTask específico.](printtask.md) |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador printTaskTrigger. Apenas leitura.|
|event|printEvent|O evento Impressão Universal que fará com que um [novo printTask](printtask.md) seja acionado. Os valores válidos são descritos na tabela a seguir.|

### <a name="printevent-values"></a>valores printEvent

|Membro|Valor|Descrição|
|:---|:---|:---|
|jobStarted|0|Representa um evento que ocorre quando um novo trabalho de impressão é iniciado.|
|unknownFutureValue|1|Valor de sentinela de enumeração evolvável. Não usar.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definition|[printTaskDefinition](printtaskdefinition.md)|Uma definição abstrata que será usada para criar [uma printTask](printtask.md) quando disparada por um evento de impressão. Somente leitura.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printTaskTrigger",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTaskTrigger",
  "id": "String (identifier)",
  "event": "String"
}
```

