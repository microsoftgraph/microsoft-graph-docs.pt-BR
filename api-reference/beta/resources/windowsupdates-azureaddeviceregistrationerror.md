---
title: Tipo de recurso azureADDeviceRegistrationError
description: Um erro no processo de registro de um dispositivo do Azure AD que impede o serviço de registrar o dispositivo no gerenciamento de atualizações ou implantar conteúdo no dispositivo.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: cd2699c4fecb694e5678d192d07c0fe2f904ee92
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61863519"
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

