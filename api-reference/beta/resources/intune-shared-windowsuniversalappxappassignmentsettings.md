---
title: Tipo de recurso windowsUniversalAppXAppAssignmentSettings
description: Contém propriedades usadas ao atribuir Windows aplicativo móvel Universal AppX a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5062e1406ed29e3d042d1351f60e4a9b411bbe8f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58769331"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a>Tipo de recurso windowsUniversalAppXAppAssignmentSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades usadas ao atribuir Windows aplicativo móvel Universal AppX a um grupo.


Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|useDeviceContext|Booliano|Se deve ou não usar o contexto de execução de dispositivos Windows aplicativo móvel Universal AppX.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUniversalAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```



