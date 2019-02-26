---
title: Tipo de recurso windowsInformationProtectionStoreApp
description: Aplicativo de loja para proteção de informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3ce294f8c22dea483f9b72b167b7ee092e339b7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142557"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a>Tipo de recurso windowsInformationProtectionStoreApp

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Aplicativo de loja para proteção de informações do Windows


Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome de exibição do aplicativo. Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|descrição|String|A descrição do aplicativo. Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|publisherName|String|O nome do fornecedor herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|productName|Cadeia de caracteres|O nome do produto. Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|negado|Booliano|Se verdadeiro, é negada proteção ou isenção ao aplicativo. Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionStoreApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```




