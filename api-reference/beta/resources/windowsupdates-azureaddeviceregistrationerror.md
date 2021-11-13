---
title: Tipo de recurso azureADDeviceRegistrationError
description: Um erro no processo de registro de um dispositivo do Azure AD que impede o serviço de registrar o dispositivo no gerenciamento de atualizações ou implantar conteúdo no dispositivo.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 8ef1d16203f4b2197a0f8cdb93aaeae073d77ccb
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890364"
---
# <a name="azureaddeviceregistrationerror-resource-type"></a>Tipo de recurso azureADDeviceRegistrationError

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um erro no processo de registro de um dispositivo [do Azure AD](../resources/windowsupdates-azureaddevice.md) que impede o serviço de registrar o dispositivo no gerenciamento de atualizações ou implantar conteúdo no dispositivo.

Herda de [updatableAssetError](../resources/windowsupdates-updatableasseterror.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|motivo|microsoft.graph.windowsUpdates.azureADDeviceRegistrationErrorReason|O motivo pelo qual o registro encontrou um erro. Os valores possíveis são: `invalidGlobalDeviceId`, `invalidAzureADDeviceId`, `missingTrustType`, `invalidAzureADJoin`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.azureADDeviceRegistrationError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.azureADDeviceRegistrationError",
  "reason": "String"
}
```

