---
title: tipo de enumeração vpnServiceExceptionAction
description: A ação VPN a ser tomada para um serviço específico.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1310d91da9a7ea8e3a6274acd48e8ebc1359cafd
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636711"
---
# <a name="vpnserviceexceptionaction-enum-type"></a>tipo de enumeração vpnServiceExceptionAction

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A ação VPN a ser tomada para um serviço específico.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|forceTrafficViaVPN|,0|Fazer com que todo o tráfego desse serviço percorra a VPN|
|allowTrafficOutside|1 |Permitir o serviço fora da VPN|
|dropTraffic|2 |Remover todo o tráfego do serviço|



