---
title: Tipo de recurso vppLicensingType
description: Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73b46c9bcd8680ffbd78c1cfc85cc6dec85126e6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256116"
---
# <a name="vpplicensingtype-resource-type"></a>Tipo de recurso vppLicensingType

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|supportsUserLicensing|Boolean|Se o programa dá suporte ao tipo de licença do usuário.|
|supportsDeviceLicensing|Booliano|Se o programa dá suporte ao tipo de licenciamento do dispositivo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



