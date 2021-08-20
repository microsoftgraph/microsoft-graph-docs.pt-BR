---
title: Tipo de recurso macOSLobChildApp
description: Contém propriedades do Aplicativo LOB do MacOS em um pacote de pacotes
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6b005b3acf933e6e12eaf0a0f0be15c4a2596b701f72ee920887e04db5ca2d12
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54213351"
---
# <a name="macoslobchildapp-resource-type"></a>Tipo de recurso macOSLobChildApp

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades do Aplicativo LOB do MacOS em um pacote de pacotes

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|bundleId|String|O Nome da Identidade.|
|buildNumber|String|O número de composição do aplicativo MacOS Line of Business (LoB).|
|versionNumber|String|O número de versão do aplicativo MacOS Line of Business (LoB).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```




