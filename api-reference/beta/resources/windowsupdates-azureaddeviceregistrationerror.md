---
title: Tipo de recurso azureADDeviceRegistrationError
description: Um erro no processo de registro de um dispositivo do Azure AD que impede o serviço de registrar o dispositivo no gerenciamento de atualizações ou implantar conteúdo no dispositivo.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 1d08ab96d5298c70f34acf89e3c6c4605d9df0a1
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067800"
---
# <a name="azureaddeviceregistrationerror-resource-type"></a>Tipo de recurso azureADDeviceRegistrationError

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um erro no processo de registro de um dispositivo [do Azure AD](../resources/windowsupdates-azureaddevice.md) que impede o serviço de registrar o dispositivo no gerenciamento de atualizações ou implantar conteúdo no dispositivo.

Herda de [updatableAssetError](../resources/windowsupdates-updatableasseterror.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|motivo|microsoft.graph.windowsUpdates.azureADDeviceRegistrationErrorReason|O motivo pelo qual o registro encontrou um erro. Os valores possíveis são: `invalidGlobalDeviceId`, `invalidAzureADDeviceId`, `missingTrustType`, `invalidAzureADJoin`.|

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

