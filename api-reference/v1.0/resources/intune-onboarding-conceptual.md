---
title: Registrar dispositivos para o gerenciamento no Intune
description: " O registro (BYOD) permite que os usuários registrem seus telefones, tablets ou computadores pessoais. O registro de dispositivo de propriedade corporativa (COD) permite cenários de gerenciamento como apagamento remoto, dispositivos compartilhados ou afinidade de usuários em um dispositivo."
localization_priority: Normal
author: davidmu1
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 171a58e82ea3e7ab76d919d1fef693f540b4f4db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448162"
---
# <a name="enroll-devices-for-management-in-intune"></a>Registrar dispositivos para o gerenciamento no Intune

Namespace: Microsoft. Graph

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.

É possível registrar dispositivos, incluindo computadores Windows, para habilitar o gerenciamento de dispositivo móvel (MDM) com o Microsoft Intune. Este tópico descreve as diferentes maneiras de registrar dispositivos móveis no gerenciamento do Intune. A maneira de registrar dispositivos depende do tipo de dispositivo, da propriedade e do nível de gerenciamento necessário. O registro "Traga seu próprio dispositivo" (BYOD) permite aos usuários registrar seus telefones, computador e tablets pessoais. O registro de dispositivo de propriedade corporativa (COD) permite cenários de gerenciamento como apagamento remoto, dispositivos compartilhados ou afinidade de usuários em um dispositivo.

Os seguintes recursos do Graph estão disponíveis para gerenciar registros no Intune:  

- [Configuração de registro do dispositivo](intune-onboarding-deviceenrollmentconfiguration.md)
- [Configuração de limite do registro do dispositivo](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [Restrição da plataforma de registro do dispositivo](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [Configuração das restrições da plataforma de registro do dispositivo](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [Configuração do Windows Hello para empresas do registro do dispositivo](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [Conector do Exchange de gerenciamento de dispositivo](intune-onboarding-devicemanagementexchangeconnector.md)
- [Status do conector do Exchange de gerenciamento de dispositivo](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [Tipo de sincronização do conector do Exchange de gerenciamento de dispositivo](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [Tipo de conector do Exchange de gerenciamento de dispositivo](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [Parceiro de gerenciamento do dispositivo](intune-onboarding-devicemanagementpartner.md)
- [Tipo de aplicativo de parceiro de gerenciamento do dispositivo](intune-onboarding-devicemanagementpartnerapptype.md)
- [Estado de locatário de parceiro de gerenciamento do dispositivo](intune-onboarding-devicemanagementpartnertenantstate.md)
- [Habilitação](intune-onboarding-enablement.md)
- [Atribuição de configuração do registro](intune-onboarding-enrollmentconfigurationassignment.md)
- [Marca Intune](intune-onboarding-intunebrand.md)
- [Autoridade MDM](intune-onboarding-mdmauthority.md)
- [Conector de defesa contra ameaças móveis](intune-onboarding-mobilethreatdefenseconnector.md)
- [Estado de locatário do parceiro de ameaças móveis](intune-onboarding-mobilethreatpartnertenantstate.md)
- [Configuração de acesso condicional local](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [Organização](intune-onboarding-organization.md)
- [Cores RGB](intune-onboarding-rgbcolor.md)
- [Token VPP](intune-onboarding-vpptoken.md)
- [Estado do token VPP](intune-onboarding-vpptokenstate.md)
- [Status de sincronização do token VPP](intune-onboarding-vpptokensyncstatus.md)
- [Uso do PIN do Windows Hello para empresas](intune-onboarding-windowshelloforbusinesspinusage.md)

