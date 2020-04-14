---
title: tipo de enumeração vpnServiceExceptionAction
description: A ação VPN a ser tomada para um serviço específico.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 125410fb9d501ec3dc205cc29c0728c7c54b007f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420221"
---
# <a name="vpnserviceexceptionaction-enum-type"></a>tipo de enumeração vpnServiceExceptionAction

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A ação VPN a ser tomada para um serviço específico.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|forceTrafficViaVPN|,0|Fazer com que todo o tráfego desse serviço percorra a VPN|
|allowTrafficOutside|1|Permitir o serviço fora da VPN|
|dropTraffic|duas|Remover todo o tráfego do serviço|



