---
title: Tipo de recurso windowsDriverUpdateInventory
description: Uma nova entidade para representar inventários de driver.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d61d8d0dbefabb0bbb2cfc2be823ff66a2ba2ae3
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58792118"
---
# <a name="windowsdriverupdateinventory-resource-type"></a>Tipo de recurso windowsDriverUpdateInventory

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma nova entidade para representar inventários de driver.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsDriverUpdateInventories](../api/intune-softwareupdate-windowsdriverupdateinventory-list.md)|[Coleção windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|Listar propriedades e relações dos [objetos windowsDriverUpdateInventory.](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|
|[Obter windowsDriverUpdateInventory](../api/intune-softwareupdate-windowsdriverupdateinventory-get.md)|[windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|Leia propriedades e relações do [objeto windowsDriverUpdateInventory.](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|
|[Criar windowsDriverUpdateInventory](../api/intune-softwareupdate-windowsdriverupdateinventory-create.md)|[windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|Crie um novo [objeto windowsDriverUpdateInventory.](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|
|[Excluir windowsDriverUpdateInventory](../api/intune-softwareupdate-windowsdriverupdateinventory-delete.md)|Nenhum(a)|Exclui um [windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md).|
|[Atualizar windowsDriverUpdateInventory](../api/intune-softwareupdate-windowsdriverupdateinventory-update.md)|[windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|Atualize as propriedades de um [objeto windowsDriverUpdateInventory.](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A id do driver.|
|nome|Cadeia de caracteres|O nome do driver.|
|versão|String|A versão do driver.|
|fabricante|String|O fabricante do driver.|
|releaseDateTime|DateTimeOffset|A data de lançamento do driver.|
|driverClass|Cadeia de caracteres|A classe do driver.|
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



