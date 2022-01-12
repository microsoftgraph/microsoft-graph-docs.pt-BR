---
title: Tipo de recurso do azureADDevice
description: Representa um dispositivo no Azure Active Directory (Azure AD) registrado no serviço de implantação.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a055c944c1b7a5f2bd4bbd23a9edc8d9c3b3ff88
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792187"
---
# <a name="azureaddevice-resource-type"></a>Tipo de recurso do azureADDevice

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um dispositivo no Azure Active Directory (Azure AD) registrado no serviço de implantação.

Um dispositivo do Azure AD é criado automaticamente por meio de um dos seguintes métodos:
* [updatableAsset: enrollAssets](../api/windowsupdates-updatableasset-enrollassets.md)
* [updatableAsset: enrollAssetsById](../api/windowsupdates-updatableasset-enrollassetsbyid.md)
* [deploymentAudience: updateAudience](../api/windowsupdates-deploymentaudience-updateaudience.md)
* [deploymentAudience: updateAudienceById](../api/windowsupdates-deploymentaudience-updateaudiencebyid.md)
* [updatableAssetGroup: addMembers](../api/windowsupdates-updatableassetgroup-addmembers.md)
* [updatableAssetGroup: addMembersById](../api/windowsupdates-updatableassetgroup-addmembersbyid.md)

Herda de [updatableAsset](../resources/windowsupdates-updatableasset.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar recursos do azureADDevice](../api/windowsupdates-updates-list-updatableassets-azureaddevice.md)|[coleção microsoft.graph.windowsUpdates.azureADDevice](../resources/windowsupdates-azureaddevice.md)|Obter uma lista dos [objetos azureADDevice](../resources/windowsupdates-azureaddevice.md) e suas propriedades.|
|[Obter azureADDevice](../api/windowsupdates-azureaddevice-get.md)|[microsoft.graph.windowsUpdates.azureADDevice](../resources/windowsupdates-azureaddevice.md)|Leia as propriedades e as relações de um [objeto azureADDevice.](../resources/windowsupdates-azureaddevice.md)|
|[Excluir azureADDevice](../api/windowsupdates-azureaddevice-delete.md)|Nenhum|[Exclua um objeto azureADDevice.](../resources/windowsupdates-azureaddevice.md)|
|[Registrar recursos do azureADDevice no gerenciamento](../api/windowsupdates-updatableasset-enrollassets.md)|Nenhum|Registrar [recursos do azureADDevice](../resources/windowsupdates-azureaddevice.md) no gerenciamento de atualizações pelo serviço de implantação.|
|[Registrar recursos do azureADDevice no gerenciamento (por ID)](../api/windowsupdates-updatableasset-enrollassetsbyid.md)|Nenhum|Registrar [recursos do azureADDevice](../resources/windowsupdates-azureaddevice.md) no gerenciamento de atualizações pelo serviço de implantação.|
|[Desembre recursos do azureADDevice do gerenciamento](../api/windowsupdates-updatableasset-unenrollassets.md)|Nenhum|Desembre [recursos do azureADDevice](../resources/windowsupdates-azureaddevice.md) do gerenciamento de atualizações pelo serviço de implantação.|
|[Desembre recursos do azureADDevice do gerenciamento (por ID)](../api/windowsupdates-updatableasset-unenrollassetsbyid.md)|Nenhum|Desembre [recursos do azureADDevice](../resources/windowsupdates-azureaddevice.md) do gerenciamento de atualizações pelo serviço de implantação.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|enrollments|[coleção microsoft.graph.windowsUpdates.updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md)|Especifica áreas do serviço em que o dispositivo está inscrito. Somente leitura. Devolvido por padrão.|
|erros|[coleção microsoft.graph.windowsUpdates.updatableAssetError](../resources/windowsupdates-updatableasseterror.md)|Especifica quaisquer erros que impeçam que o dispositivo seja inscrito no gerenciamento de atualizações ou receving conteúdo implantado. Somente leitura. Devolvido por padrão.|
|id|String|Um identificador do dispositivo. Chave. Não anulável. Somente leitura. Devolvido por padrão. Herdado [de updatableAsset](../resources/windowsupdates-updatableasset.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.azureADDevice",
  "baseType": "microsoft.graph.windowsUpdates.updatableAsset",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
  "id": "String (identifier)",
  "errors": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.azureADDeviceRegistrationError"
    }
  ],
  "enrollments": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment"
    }
  ]
}
```

