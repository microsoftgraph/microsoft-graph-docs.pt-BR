---
title: tipo de recurso de multiconnector
description: Representa um conector de impressão que foi registrado usando uma assinatura de impressão universal. O recurso Print Connector pode ser usado para exibir o status do conector e propriedades de atualização.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 7c66933c381e2f7563f4666ca788d06970b04490
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895506"
---
# <a name="printconnector-resource-type"></a>tipo de recurso de multiconnector

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um conector de impressão que foi registrado usando uma assinatura de impressão universal. O recurso Print Connector pode ser usado para exibir o status do conector e propriedades de atualização.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter conector](../api/printconnector-get.md) | [separador de Hiperligação](printconnector.md) | Leia as propriedades e as relações do objeto Connector. |
| [Conector de atualização](../api/printconnector-update.md) | [separador de Hiperligação](printconnector.md) | Atualize o objeto Connector. |
| [Excluir conector](../api/printconnector-delete.md) | Nenhum | Cancele o registro do conector do serviço de impressão universal. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Somente leitura.|
|name|String|O nome do conector.|
|Nomededomíniototalmentequalificado|String|O nome de host do computador do conector.|
|operatingSystem|String|A versão do sistema operacional do computador do conector.|
|appVersion|String|A versão do conector.|
|deviceHealth|[deviceHealth](devicehealth.md)|A integridade do dispositivo do conector.|
|location|[printerLocation](printerlocation.md)|O local físico e/ou organizacional do conector.|
|registeredDateTime|DateTimeOffset|O DateTimeOffset quando o conector foi registrado.|
|registeredBy|[userIdentity](useridentity.md)|O usuário que registrou o conector.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printConnector"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "fullyQualifiedDomainName": "String",
  "operatingSystem": "String",
  "appVersion": "String",
  "deviceHealth": {"@odata.type": "microsoft.graph.deviceHealth"},
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "registeredDateTime": "String (timestamp)",
  "registeredBy": {"@odata.type": "microsoft.graph.userIdentity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printConnector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->