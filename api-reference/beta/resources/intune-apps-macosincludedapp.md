---
title: Tipo de recurso macOSIncludedApp
description: Contém propriedades de um .app incluído em um aplicativo MacOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 87c7d8b5cc5eb1229b9860fe8192b0cd765c33c5
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/04/2022
ms.locfileid: "61712140"
---
# <a name="macosincludedapp-resource-type"></a>Tipo de recurso macOSIncludedApp

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades de um .app incluído em um aplicativo MacOS.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|bundleId|String|O CFBundleIdentifier.|
|bundleVersion|String|O CFBundleVersion.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSIncludedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSIncludedApp",
  "bundleId": "String",
  "bundleVersion": "String"
}
```




