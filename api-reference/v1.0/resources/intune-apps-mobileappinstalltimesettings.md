---
title: Tipo de recurso mobileAppInstallTimeSettings
description: Contém propriedades usadas para determinar quando oferecer um aplicativo para dispositivos e quando instalar o aplicativo em dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 147311668116b670bf62d0f2f0240f479b43089150d2d9df1c3e398a1de715dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205805"
---
# <a name="mobileappinstalltimesettings-resource-type"></a>Tipo de recurso mobileAppInstallTimeSettings

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades usadas para determinar quando oferecer um aplicativo para dispositivos e quando instalar o aplicativo em dispositivos.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|useLocalTime|Booliano|Se a hora do dispositivo local ou utc deve ser usada ao determinar os tempos disponíveis e de prazo.|
|startDateTime|DateTimeOffset|O momento em que o aplicativo deve estar disponível para instalação.|
|deadlineDateTime|DateTimeOffset|O momento em que o aplicativo deve ser instalado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallTimeSettings",
  "useLocalTime": true,
  "startDateTime": "String (timestamp)",
  "deadlineDateTime": "String (timestamp)"
}
```




