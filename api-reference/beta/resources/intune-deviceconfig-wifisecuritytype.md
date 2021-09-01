---
title: Tipo de número wiFiSecurityType
description: Wi-Fi Tipos de Segurança.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a259b72691654ac979f65cbe4f445578743a491c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58797877"
---
# <a name="wifisecuritytype-enum-type"></a>Tipo de número wiFiSecurityType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Wi-Fi Tipos de Segurança.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|open|0|Open (Sem Autenticação).|
|wpaPersonal|1|WPA-Personal.|
|wpaEnterprise|2|WPA-Enterprise. Deve usar o tipo IOSEnterpriseWifiConfiguration para configurar as opções corporativas.|
|wep|3|Criptografia WEP.|
|wpa2Personal|4 |WPA2-Personal.|
|wpa2Enterprise|5 |WPA2-Enterprise. Deve usar o tipo WindowsWifiEnterpriseEAPConfiguration para configurar as opções corporativas.|



