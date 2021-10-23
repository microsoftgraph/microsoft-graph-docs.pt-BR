---
title: Tipo de recurso printConnector
description: Representa um conector de impressão que foi registrado usando uma assinatura de Impressão Universal. O recurso printConnector pode ser usado para exibir o status do conector e atualizar as propriedades.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: ad4a8f733f39490bbf126d60fe193a664b06888a
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561770"
---
# <a name="printconnector-resource-type"></a>Tipo de recurso printConnector

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um conector de impressão que foi registrado usando uma assinatura de Impressão Universal. O recurso printConnector pode ser usado para exibir o status do conector e atualizar as propriedades.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar conectores](../api/print-list-connectors.md) | [printConnector](printconnector.md) | Recupere uma lista de conectores de impressão. |
| [Obter conector](../api/printconnector-get.md) | [printConnector](printconnector.md) | Leia as propriedades e as relações do objeto conector. |
| [Conector de atualização](../api/printconnector-update.md) | [printConnector](printconnector.md) | Atualize o objeto connector. |
| [Excluir conector](../api/printconnector-delete.md) | Nenhum | Desaconselhe o conector do serviço de Impressão Universal. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Somente leitura.|
|displayName|Cadeia de caracteres|O nome do conector.|
|fullyQualifiedDomainName|Cadeia de Caracteres|O nome de host do computador do conector.|
|operatingSystem|String|A versão do sistema operacional do conector.|
|appVersion|Cadeia de Caracteres|A versão do conector.|
|deviceHealth|[deviceHealth](devicehealth.md)|A saúde do dispositivo do conector.|
|localização|[printerLocation](printerlocation.md)|O local físico e/ou organizacional do conector.|
|registeredDateTime|DateTimeOffset|DateTimeOffset quando o conector foi registrado.|
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
  "displayName": "String",
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


