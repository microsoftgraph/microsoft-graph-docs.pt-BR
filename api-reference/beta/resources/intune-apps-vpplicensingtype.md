---
title: Tipo de recurso vppLicensingType
description: Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6eca0f098d29d217e378ada2dcc85535eb39283b67b43fb1ac184f4b73fb9ff3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54227621"
---
# <a name="vpplicensingtype-resource-type"></a>Tipo de recurso vppLicensingType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|supportUserLicensing|Booliano|Se o programa dá suporte ao tipo de licença do usuário.|
|supportDeviceLicensing|Booliano|Se o programa dá suporte ao tipo de licenciamento do dispositivo.|
|supportsUserLicensing|Booliano|Se o programa dá suporte ao tipo de licença do usuário.|
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
  "supportUserLicensing": true,
  "supportDeviceLicensing": true,
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```




