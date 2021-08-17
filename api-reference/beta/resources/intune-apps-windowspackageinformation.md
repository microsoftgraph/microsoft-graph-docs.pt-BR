---
title: Tipo de recurso windowsPackageInformation
description: Contém propriedades para as informações do pacote para um Windows de linha de negócios.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 62e408154f601f98fec33435e8b4728f3d135526
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58253499"
---
# <a name="windowspackageinformation-resource-type"></a>Tipo de recurso windowsPackageInformation

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para as informações do pacote para um Windows de linha de negócios.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|applicableArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|A Windows arquitetura para a qual este aplicativo pode ser executado. Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.|
|displayName|Cadeia de caracteres|O Nome para Exibição.|
|identityName|String|O Nome da Identidade.|
|identityPublisher|Cadeia de caracteres|A identidade Publisher.|
|identityResourceIdentifier|String|O Identificador de Recurso da Identidade.|
|identityVersion|String|A Versão de Identidade.|
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
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true,
    "v10_1909": true,
    "v10_2004": true,
    "v10_2H20": true,
    "v10_21H1": true
  }
}
```




