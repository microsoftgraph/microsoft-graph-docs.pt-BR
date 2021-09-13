---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7863eb4e0926490acfd9f064a7b21c719ab3f923
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039711"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a>Tipo de recurso deviceEnrollmentPlatformRestriction

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Restrições de registro específicas de plataformas

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|platformBlocked|Booliano|Bloqueia o registro da plataforma|
|personalDeviceEnrollmentBlocked|Booliano|Bloqueia o registro de dispositivos de sua propriedade|
|osMinimumVersion|Cadeia de caracteres|Versão do SO mínimo compatível|
|osMaximumVersion|Cadeia de caracteres|Versão do SO máximo compatível|
|blockedManufacturers|String collection|Coleção de fabricantes bloqueados.|
|blockedSkus|String collection|Coleção de Skus bloqueados.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "blockedManufacturers": [
    "String"
  ],
  "blockedSkus": [
    "String"
  ]
}
```



