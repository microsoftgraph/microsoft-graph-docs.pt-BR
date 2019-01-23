---
title: tipo de recurso de macOSFirewallApplication
description: Representa um aplicativo na lista de aplicativos de firewall macOS
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fe3bbd83c3101420ec011fda85304fabce06daf0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404208"
---
# <a name="macosfirewallapplication-resource-type"></a>tipo de recurso de macOSFirewallApplication

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Representa um aplicativo na lista de aplicativos de firewall macOS

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|bundleId|String|BundleId do aplicativo.|
|allowsIncomingConnections|Boolean|Ou não são permitidas conexões de entrada.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSFirewallApplication"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSFirewallApplication",
  "bundleId": "String",
  "allowsIncomingConnections": true
}
```




