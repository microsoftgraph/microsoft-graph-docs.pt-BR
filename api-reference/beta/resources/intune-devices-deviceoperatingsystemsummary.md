---
title: Tipo de recurso deviceOperatingSystemSummary
description: Resumo do sistema operacional do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de94b00a1660dc874e457d20315df2f3b0690164
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444480"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a>Tipo de recurso deviceOperatingSystemSummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Resumo do sistema operacional do dispositivo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|androidCount|Int32|Número da contagem de dispositivos Android.|
|iosCount|Int32|Número da contagem de dispositivo iOS.|
|macOSCount|Int32|Número da contagem de dispositivos Mac OS X.|
|windowsMobileCount|Int32|Número da contagem de dispositivos móveis Windows.|
|windowsCount|Int32|Número da contagem de dispositivos Windows.|
|unknownCount|Int32|Número da contagem de dispositivos desconhecidos.|
|androidDedicatedCount|Int32|Número de dispositivos Android dedicados.|
|androidDeviceAdminCount|Int32|Número de dispositivos do administrador de dispositivos Android.|
|androidFullyManagedCount|Int32|Número de dispositivos Android totalmente gerenciados.|
|androidWorkProfileCount|Int32|Número de dispositivos Android de perfil de trabalho.|
|androidCorporateWorkProfileCount|Int32|A contagem de dispositivos Android de perfil de trabalho corporativo. Também conhecido como Propriedade Corporativa Habilitada Pessoalmente (COPE). Valores válidos -1 a 2147483647|
|configMgrDeviceCount|Int32|Número de dispositivos gerenciados configMgr.|
|aospUserlessCount|Int32|Número de dispositivos Android sem usuário AOSP. Valores válidos de 0 a 2147483647|
|aospUserAssociatedCount|Int32|Número de dispositivos Android associados ao usuário AOSP. Valores válidos de 0 a 2147483647|
|linuxCount|Int32|Número de dispositivos do sistema operacional Linux. Valores válidos de 0 a 2147483647|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024,
  "androidDedicatedCount": 1024,
  "androidDeviceAdminCount": 1024,
  "androidFullyManagedCount": 1024,
  "androidWorkProfileCount": 1024,
  "androidCorporateWorkProfileCount": 1024,
  "configMgrDeviceCount": 1024,
  "aospUserlessCount": 1024,
  "aospUserAssociatedCount": 1024,
  "linuxCount": 1024
}
```




