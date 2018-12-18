---
title: tipo de recurso de managedDeviceReportedApp
description: Dados de aplicativo para relatórios
author: tfitzmac
ms.openlocfilehash: 7fd01c5fd7553769653abd6e16ecc9ec40a79b8a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359490"
---
# <a name="manageddevicereportedapp-resource-type"></a>tipo de recurso de managedDeviceReportedApp

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Dados de aplicativo para relatórios
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appId|Cadeia de caracteres|O aplicativo ou identificador do pacote do aplicativo|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceReportedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceReportedApp",
  "appId": "String"
}
```





