---
title: Tipo de recurso windowsDriverUpdateInventory
description: Uma nova entidade para representar inventários de driver.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: be31bcdc9193e6bbd62c0b5a2bca0e0d939bf530
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61343599"
---
# <a name="windowsdriverupdateinventory-resource-type"></a>Tipo de recurso windowsDriverUpdateInventory

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma nova entidade para representar inventários de driver.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsDriverUpdateInventories](../api/intune-softwareupdate-windowsdriverupdateinventory-list.md)|[Coleção windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|Listar propriedades e relações dos [objetos windowsDriverUpdateInventory.](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|
|[Obter windowsDriverUpdateInventory](../api/intune-softwareupdate-windowsdriverupdateinventory-get.md)|[windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|Leia propriedades e relações do [objeto windowsDriverUpdateInventory.](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|
|[Criar windowsDriverUpdateInventory](../api/intune-softwareupdate-windowsdriverupdateinventory-create.md)|[windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|Crie um novo [objeto windowsDriverUpdateInventory.](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|
|[Excluir windowsDriverUpdateInventory](../api/intune-softwareupdate-windowsdriverupdateinventory-delete.md)|Nenhum|Exclui um [windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md).|
|[Atualizar windowsDriverUpdateInventory](../api/intune-softwareupdate-windowsdriverupdateinventory-update.md)|[windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|Atualize as propriedades de um [objeto windowsDriverUpdateInventory.](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A id do driver.|
|nome|String|O nome do driver.|
|versão|String|A versão do driver.|
|fabricante|String|O fabricante do driver.|
|releaseDateTime|DateTimeOffset|A data de lançamento do driver.|
|driverClass|String|A classe do driver.|
|applicableDeviceCount|Int32|O número de dispositivos para os quais esse driver é aplicável.|
|approvalStatus|[driverApprovalStatus](../resources/intune-softwareupdate-driverapprovalstatus.md)|O status de aprovação desse driver. Os valores possíveis são: `needsReview`, `declined`, `approved`, `suspended`.|
|category|[driverCategory](../resources/intune-softwareupdate-drivercategory.md)|A categoria desse driver. Os valores possíveis são: `recommended`, `previouslyApproved`, `other`.|
|deployDateTime|DateTimeOffset|A data em que um driver deve ser implantado se approvalStatus for aprovado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDriverUpdateInventory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDriverUpdateInventory",
  "id": "String (identifier)",
  "name": "String",
  "version": "String",
  "manufacturer": "String",
  "releaseDateTime": "String (timestamp)",
  "driverClass": "String",
  "applicableDeviceCount": 1024,
  "approvalStatus": "String",
  "category": "String",
  "deployDateTime": "String (timestamp)"
}
```




