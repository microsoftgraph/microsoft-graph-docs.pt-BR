---
title: Tipo de recurso deviceExchangeAccessStateSummary
description: Resumo do Estado de Acesso ao Exchange do dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4bf29cf514e9d2915957ffb18dc618425d326751
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000008"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a>Tipo de recurso deviceExchangeAccessStateSummary

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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





