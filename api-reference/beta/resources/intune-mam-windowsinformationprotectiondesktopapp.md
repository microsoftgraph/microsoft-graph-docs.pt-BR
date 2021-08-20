---
title: Tipo de recurso windowsInformationProtectionDesktopApp
description: Aplicativo da área de trabalho para a proteção de informações do Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 39abbcd348f6d2f781611f91aeb0a5a1b329e11483e93baa277d9b3278755d6c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54219791"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a>Tipo de recurso windowsInformationProtectionDesktopApp

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Aplicativo da área de trabalho para a proteção de informações do Windows


Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome de exibição do aplicativo. Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|description|Cadeia de caracteres|A descrição do aplicativo. Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|publisherName|String|O nome do fornecedor herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
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




