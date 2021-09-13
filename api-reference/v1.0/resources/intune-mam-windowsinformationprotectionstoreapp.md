---
title: Tipo de recurso windowsInformationProtectionStoreApp
description: Aplicativo de loja para proteção de informações do Windows
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7d2370daf066bbd96a7b7245129734e66228e5f9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044570"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a>Tipo de recurso windowsInformationProtectionStoreApp

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Aplicativo de loja para proteção de informações do Windows


Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome de exibição do aplicativo. Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|description|String|A descrição do aplicativo. Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
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




