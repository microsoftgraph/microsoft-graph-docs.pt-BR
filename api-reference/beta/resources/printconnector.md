---
title: tipo de recurso de multiconnector
description: Representa um conector de impressão que foi registrado usando uma assinatura de impressão universal. O recurso Print Connector pode ser usado para exibir o status do conector e propriedades de atualização.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 84c9625bd8d5a454100cab166676c1dcbcfd8d05
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142425"
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
| [Excluir conector](../api/printconnector-delete.md) | Nenhuma | Cancele o registro do conector do serviço de impressão universal. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Somente leitura.|
|name|Cadeia de caracteres|O nome do conector.|
|Nomededomíniototalmentequalificado|Cadeia de caracteres|O nome de host do computador do conector.|
|operatingSystem|String|A versão do sistema operacional do computador do conector.|
|appVersion|Cadeia de caracteres|A versão do conector.|
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
