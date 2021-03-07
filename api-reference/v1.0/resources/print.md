---
title: tipo de recurso de impressão
description: Quando acompanhado por uma assinatura de Impressão Universal, o recurso Imprimir permite o gerenciamento de impressoras e a descoberta de printServiceEndpoints que podem ser usados para gerenciar impressoras e trabalhos de impressão no Universal Print.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: db532fed1bcdeeec749d59c8297fc36d836aed78
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516917"
---
# <a name="print-resource-type"></a>tipo de recurso de impressão

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Quando acompanhado por uma assinatura de Impressão Universal, o recurso Imprimir permite o gerenciamento de impressoras e a descoberta de [printServiceEndpoints](printserviceendpoint.md) que podem ser usados para gerenciar impressoras e trabalhos de impressão no Universal Print.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [Listar conectores](../api/print-list-connectors.md) | [Coleção printConnector](printconnector.md) | Obter uma lista de conectores de impressão. |
| [Lista de impressoras](../api/print-list-printers.md) | [coleção printer](printer.md) | Obter uma lista de impressoras. |
| [Listar shares](../api/print-list-shares.md) | [Coleção printerShare](printershare.md) | Obter uma lista de compartilhamentos de impressora. |
| [Listar serviços](../api/print-list-services.md) | [Coleção printService](printservice.md) | Obter uma lista de serviços. |
| [Criar printerShare](../api/print-post-shares.md) | [printerShare](printershare.md) | Crie um novo compartilhamento de impressora postando na coleção **de compartilhamentos.** |
| [Criar impressora](../api/printer-create.md) | [printerCreateOperation](printerCreateOperation.md) | Criar (registrar) uma nova impressora com Impressão Universal. |
| [Atualizar configurações](../api/print-update-settings.md) |  [printSettings](printsettings.md) | Atualiza as configurações de todo o locatário para o serviço de Impressão Universal. |
| [Listar taskDefinitions](../api/print-list-taskdefinitions.md) | [Coleção printTaskDefinition](printtaskdefinition.md) | Obter uma lista em todo o locatário de printTaskDefinitions criada em Impressão Universal. |
| [Criar taskDefinition](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | Crie uma nova printTaskDefinition. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|settings|[printSettings](../resources/printsettings.md)|Configurações em todo o locatário para o serviço de Impressão Universal.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|services|[Coleção printService](printservice.md)|A lista de pontos de extremidade de serviço de Impressão Universal disponíveis.|
|impressoras|[coleção printer](printer.md)|A lista de impressoras registradas no locatário.|
|shares|[Coleção printerShare](printershare.md)|A lista de compartilhamentos de impressora registrados no locatário.|
|conectores|[Coleção printConnector](printconnector.md)|A lista de conectores de impressão disponíveis.|
|operations|[Coleção printOperation](../resources/printoperation.md)|A lista de operações de longa execução de impressão.|
|services|[Coleção printService](../resources/printservice.md)|A lista de instâncias de serviço de impressão para vários componentes da infraestrutura de impressão.|
|taskDefinitions|[Coleção printTaskDefinition](../resources/printtaskdefinition.md)|Lista de definição abstrata para uma tarefa que pode ser disparada quando vários eventos ocorrem em Impressão Universal.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.print",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.print",
  "settings": {
    "@odata.type": "microsoft.graph.printSettings"
  }
}
```

