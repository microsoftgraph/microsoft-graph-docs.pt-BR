---
title: tipo de recurso de multiconnector
description: Representa um conector de impressão que foi registrado usando uma assinatura de impressão universal. O recurso Print Connector pode ser usado para exibir o status do conector e propriedades de atualização.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: d027344db67a26fc0af7ebffaaad63d3fe3c4971
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046805"
---
# <a name="printconnector-resource-type"></a>tipo de recurso de multiconnector

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um conector de impressão que foi registrado usando uma assinatura de impressão universal. O recurso Print Connector pode ser usado para exibir o status do conector e propriedades de atualização.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter conector](../api/printconnector-get.md) | [separador de Hiperligação](printconnector.md) | Leia as propriedades e as relações do objeto Connector. |
| [Conector de atualização](../api/printconnector-update.md) | [separador de Hiperligação](printconnector.md) | Atualize o objeto Connector. |
| [Excluir conector](../api/printconnector-delete.md) | Nenhum | Cancele o registro do conector do serviço de impressão universal. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Somente leitura.|
|name|Cadeia de caracteres|O nome do conector.|
|Nomededomíniototalmentequalificado|Cadeia de caracteres|O nome de host do computador do conector.|
|operatingSystem|String|A versão do sistema operacional do computador do conector.|
|appVersion|Cadeia de caracteres|A versão do conector.|
|deviceHealth|[deviceHealth](devicehealth.md)|A integridade do dispositivo do conector.|
|localização|[printerLocation](printerlocation.md)|O local físico e/ou organizacional do conector.|
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


