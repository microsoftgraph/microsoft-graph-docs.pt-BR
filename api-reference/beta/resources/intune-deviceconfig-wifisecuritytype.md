---
title: Tipo de número wiFiSecurityType
description: Wi-Fi Tipos de Segurança.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b24b05396a5b436d2c029cfe3991ccbab8cfbce665088d2f67ca62629f7d85c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251411"
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
|wpaPersonal|1 |WPA-Personal.|
|wpaEnterprise|2|WPA-Enterprise. Deve usar o tipo IOSEnterpriseWifiConfiguration para configurar as opções corporativas.|
|wep|3 |Criptografia WEP.|
|wpa2Personal|4 |WPA2-Personal.|
|wpa2Enterprise|5 |WPA2-Enterprise. Deve usar o tipo WindowsWifiEnterpriseEAPConfiguration para configurar as opções corporativas.|




