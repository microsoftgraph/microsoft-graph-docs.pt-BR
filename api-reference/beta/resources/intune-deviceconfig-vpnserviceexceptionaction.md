---
title: Tipo de número vpnServiceExceptionAction
description: A ação VPN a ser tomada para um serviço específico.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a43e97e993a9a605aee3561c188bf3a969f0510d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59027075"
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



