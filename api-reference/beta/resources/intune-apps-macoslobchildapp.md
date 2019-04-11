---
title: tipo de recurso macOSLobChildApp
description: Contém as propriedades do aplicativo de LOB do MacOS em um pacote de pacote
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54bd15c4549495ff891d7283c6851e7058ffb887
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780207"
---
# <a name="macoslobchildapp-resource-type"></a>tipo de recurso macOSLobChildApp

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém as propriedades do aplicativo de LOB do MacOS em um pacote de pacote

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|bundleId|String|O Nome da Identidade.|
|buildNumber|String|O número de compilação do aplicativo de linha de negócios (LoB) MacOS.|
|versionNumber|Cadeia de caracteres|O número da versão do aplicativo de linha de negócios (LoB) MacOS.|

## <a name="relationships"></a>Relações
Nenhuma

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





