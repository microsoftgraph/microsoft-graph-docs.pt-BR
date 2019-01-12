---
title: tipo de recurso de windowsPackageInformation
description: Contém propriedades para as informações de pacote para uma linha do Windows do aplicativo de negócios.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac0f9aad1cdba1eaaac12754fd4a4d0ad4a6db32
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926845"
---
# <a name="windowspackageinformation-resource-type"></a>tipo de recurso de windowsPackageInformation

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades para as informações de pacote para uma linha do Windows do aplicativo de negócios.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|applicableArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|A arquitetura do Windows para a qual este aplicativo pode executar em. Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.|
|displayName|Cadeia de caracteres|O nome de exibição.|
|identityName|Cadeia de caracteres|O Nome da Identidade.|
|identityPublisher|Cadeia de caracteres|O Editor de identidade.|
|identityResourceIdentifier|Cadeia de caracteres|O Identificador de Recurso da Identidade.|
|identityVersion|Cadeia de caracteres|A versão de identidade.|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune-apps-windowsminimumoperatingsystem.md)|O valor do sistema de operacional mínimo aplicável.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsPackageInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPackageInformation",
  "applicableArchitecture": "String",
  "displayName": "String",
  "identityName": "String",
  "identityPublisher": "String",
  "identityResourceIdentifier": "String",
  "identityVersion": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  }
}
```





