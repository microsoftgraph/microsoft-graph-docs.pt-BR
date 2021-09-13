---
title: Tipo de número wiFiSecurityType
description: Wi-Fi Tipos de Segurança.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 600173712b5e00f8af9a6e9a94dc4b2167d6130b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057373"
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



