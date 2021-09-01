---
title: Tipo de número vpnServiceExceptionAction
description: A ação VPN a ser tomada para um serviço específico.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 851292848633b17600228869e305b4504223dc96
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783943"
---
# <a name="vpnserviceexceptionaction-enum-type"></a>Tipo de número vpnServiceExceptionAction

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A ação VPN a ser tomada para um serviço específico.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|forceTrafficViaVPN|0|Fazer todo o tráfego desse serviço passar pela VPN|
|allowTrafficOutside|1|Permitir o serviço fora da VPN|
|dropTraffic|2|Soltar todo o tráfego do serviço|



