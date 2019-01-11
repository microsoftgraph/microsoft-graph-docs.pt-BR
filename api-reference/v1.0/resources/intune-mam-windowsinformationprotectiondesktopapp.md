---
title: Tipo de recurso windowsInformationProtectionDesktopApp
description: Aplicativo da área de trabalho para a proteção de informações do Windows
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c381541379feacff7611e77882069c5fe2119e67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822061"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a>Tipo de recurso windowsInformationProtectionDesktopApp

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Aplicativo da área de trabalho para a proteção de informações do Windows

Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome de exibição do aplicativo. Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|descrição|Cadeia de caracteres|A descrição do aplicativo. Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|publisherName|Cadeia de caracteres|O nome do fornecedor herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|productName|Cadeia de caracteres|O nome do produto. Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|negado|Booliano|Se verdadeiro, é negada proteção ou isenção ao aplicativo. Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|binaryName|Cadeia de caracteres|O nome binário.|
|binaryVersionLow|Cadeia de caracteres|A versão binária inferior.|
|binaryVersionHigh|Cadeia de caracteres|A versão binária superior.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDesktopApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true,
  "binaryName": "String",
  "binaryVersionLow": "String",
  "binaryVersionHigh": "String"
}
```



