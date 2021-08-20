---
title: Tipo de recurso deviceExchangeAccessStateSummary
description: Resumo do Estado de Acesso ao Exchange do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c964a3ca125e50672087484e7ea7fc2321ad645a2268058f854a8701894a3d58
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54185723"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a>Tipo de recurso deviceExchangeAccessStateSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Resumo do Estado de Acesso ao Exchange do dispositivo

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedDeviceCount|Int32|Contagem total de dispositivos com Estado de Acesso ao Exchange: Permitido.|
|blockedDeviceCount|Int32|Contagem total de dispositivos com Estado de Acesso ao Exchange: Bloqueado.|
|quarantinedDeviceCount|Int32|Contagem total de dispositivos com Estado de Acesso ao Exchange: Em quarentena.|
|unknownDeviceCount|Int32|Contagem total de dispositivos com Estado de Acesso ao Exchange: Desconhecido.|
|unavailableDeviceCount|Int32|Contagem total de dispositivos para os quais nenhum Estado de Acesso ao Exchange pôde ser encontrado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": 1024,
  "blockedDeviceCount": 1024,
  "quarantinedDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "unavailableDeviceCount": 1024
}
```




