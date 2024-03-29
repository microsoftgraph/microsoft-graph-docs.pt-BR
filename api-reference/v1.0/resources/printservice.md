---
title: Tipo de recurso printService
description: Representa uma descrição específica do locatário do Azure AD de uma instância de serviço de impressão. Os serviços existem para cada componente da infraestrutura de impressão (por exemplo, descoberta, notificações, registro e IPP) e têm um ou mais pontos de extremidade.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 7319ee78846f98f0d41faab9deecff6bc2b1830b
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60936954"
---
# <a name="printservice-resource-type"></a>Tipo de recurso printService

Namespace: microsoft.graph

Representa uma descrição específica do locatário do Azure AD de uma instância de serviço de impressão. Os serviços existem para cada componente da infraestrutura de impressão (descoberta, notificações, registro e IPP) e têm um ou mais pontos de extremidade.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [Listar serviços](../api/print-list-services.md) | [Coleção printService](printservice.md) | Obter uma lista de serviços de Impressão Universal. |
| [Obter serviço](../api/printservice-get.md) | [printService](printservice.md) | Leia as propriedades e as relações do objeto service. |
| [Listar pontos de extremidade](../api/printservice-list-endpoints.md) | [Coleção printServiceEndpoint](printserviceendpoint.md) | Obter uma lista de pontos de extremidade que um serviço fornece. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador do serviço. Somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|pontos de extremidade|[Coleção printServiceEndpoint](printserviceendpoint.md)| Pontos de extremidade que podem ser usados para acessar o serviço. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printService",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printService",
  "id": "String (identifier)"
}
```

