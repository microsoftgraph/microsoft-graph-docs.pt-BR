---
title: Tipo de recurso iosMinimumOperatingSystem
description: Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0e7504cb4b4ff666bf7d40bdbfaf457fb6b812f9a3b3ee9f4e6e53cd0c63eeb8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54165893"
---
# <a name="iosminimumoperatingsystem-resource-type"></a>Tipo de recurso iosMinimumOperatingSystem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|v8_0|Booliano|Versão 8.0 ou posterior.|
|v9_0|Booliano|Versão 9.0 ou posterior.|
|v10_0|Booliano|Versão 10.0 ou posterior.|
|v11_0|Booliano|Versão 11.0 ou posterior.|
|v12_0|Boolean|Versão 12.0 ou posterior.|
|v13_0|Boolean|Versão 13.0 ou posterior.|
|v14_0|Boolean|Versão 14.0 ou posterior.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true,
  "v12_0": true,
  "v13_0": true,
  "v14_0": true
}
```




