---
title: Tipo de recurso printConnector
description: Representa um conector de impressão que foi registrado usando uma assinatura de Impressão Universal. O recurso printConnector pode ser usado para exibir o status do conector e atualizar as propriedades.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: ab2f1718837c88af61e0e790acb2ad198cfded32
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60560041"
---
# <a name="printconnector-resource-type"></a>Tipo de recurso printConnector

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Representa um conector de impressão que foi registrado usando uma assinatura de Impressão Universal. O recurso printConnector pode ser usado para exibir o status do conector e atualizar as propriedades.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [Listar conectores](../api/print-list-connectors.md) | [printConnector](printconnector.md) | Recupere uma lista de conectores de impressão. |
| [Obter conector](../api/printconnector-get.md) | [printConnector](printconnector.md) | Leia as propriedades e as relações do objeto conector. |
| [Conector de atualização](../api/printconnector-update.md) | [printConnector](printconnector.md) | Atualize o objeto connector. |
| [Excluir conector](../api/printconnector-delete.md) | Nenhum | Desaconselhe o conector do serviço de Impressão Universal. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String| Somente leitura.|
|displayName|Cadeia de caracteres|O nome do conector.|
|fullyQualifiedDomainName|Cadeia de Caracteres|O nome de host do computador do conector.|
|operatingSystem|String|A versão do sistema operacional do conector.|
|appVersion|Cadeia de Caracteres|A versão do conector.|
|localização|[printerLocation](printerlocation.md)|O local físico e/ou organizacional do conector.|
|registeredDateTime|DateTimeOffset|DateTimeOffset quando o conector foi registrado.|
|registeredBy|[userIdentity](useridentity.md)|O usuário que registrou o conector.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printConnector",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "fullyQualifiedDomainName": "String",
  "operatingSystem": "String",
  "appVersion": "String",
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "registeredDateTime": "String (timestamp)"
}
```
