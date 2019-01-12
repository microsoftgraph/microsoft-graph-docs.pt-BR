---
title: tipo de enum wiFiSecurityType
description: Tipos de segurança Wi-Fi.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6ddadaa31febaea08050ad49ffa540de53ff4819
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920216"
---
# <a name="wifisecuritytype-enum-type"></a>tipo de enum wiFiSecurityType

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Tipos de segurança Wi-Fi.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Abrir|0|Abra (nenhuma autenticação).|
|wpaPersonal|1|WPA-Pessoal.|
|wpaEnterprise|2|WPA-Empresa. Deve usar o tipo de IOSEnterpriseWifiConfiguration para configurar opções da empresa.|
|WEP|3|Criptografia WEP.|
|wpa2Personal|4|WPA2-pessoal.|
|wpa2Enterprise|5|WPA2-Empresa. Deve usar o tipo de WindowsWifiEnterpriseEAPConfiguration para configurar opções da empresa.|





