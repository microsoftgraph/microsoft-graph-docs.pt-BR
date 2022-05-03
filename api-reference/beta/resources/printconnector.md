---
title: Tipo de recurso printConnector
description: Representa um conector de impressão que foi registrado usando uma assinatura de Impressão Universal. O recurso printConnector pode ser usado para exibir o status do conector e atualizar as propriedades.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: c482d17cd702751f5f2cd2b8cff5e34166fb2075
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176907"
---
# <a name="printconnector-resource-type"></a>Tipo de recurso printConnector

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um conector de impressão que foi registrado usando uma assinatura de Impressão Universal. O recurso printConnector pode ser usado para exibir o status do conector e atualizar as propriedades.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar conectores](../api/print-list-connectors.md) | [printConnector](printconnector.md) | Recuperar uma lista de conectores de impressão. |
| [Obter conector](../api/printconnector-get.md) | [printConnector](printconnector.md) | Leia as propriedades e as relações do objeto do conector. |
| [Atualizar conector](../api/printconnector-update.md) | [printConnector](printconnector.md) | Atualize o objeto do conector. |
| [Excluir conector](../api/printconnector-delete.md) | Nenhum | Cancele o registro do conector do serviço de Impressão Universal. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Somente leitura.|
|displayName|Cadeia de caracteres|O nome do conector.|
|fullyQualifiedDomainName|Cadeia de Caracteres|O nome do host do computador do conector.|
|operatingSystem|String|A versão do sistema operacional do computador conector.|
|appVersion|Cadeia de Caracteres|A versão do conector.|
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


