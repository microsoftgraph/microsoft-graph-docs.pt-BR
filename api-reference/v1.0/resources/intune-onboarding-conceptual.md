---
title: Registrar dispositivos para o gerenciamento no Intune
description: " Inscrição (BYOD) permite que os usuários registrar seus telefones pessoais, tablets ou PCs. O registro de dispositivo de propriedade corporativa (COD) permite cenários de gerenciamento como apagamento remoto, dispositivos compartilhados ou afinidade de usuários em um dispositivo."
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 2e7f6e85e32137804556c64a1995bd2e78b04068
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917437"
---
# <a name="enroll-devices-for-management-in-intune"></a>Registrar dispositivos para o gerenciamento no Intune

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.

É possível registrar dispositivos, incluindo computadores Windows, para habilitar o gerenciamento de dispositivo móvel (MDM) com o Microsoft Intune. Este tópico descreve as diferentes maneiras de registrar dispositivos móveis no gerenciamento do Intune. A maneira de registrar dispositivos depende do tipo de dispositivo, da propriedade e do nível de gerenciamento necessário. O registro "Traga seu próprio dispositivo" (BYOD) permite aos usuários registrar seus telefones, computador e tablets pessoais. O registro de dispositivo de propriedade corporativa (COD) permite cenários de gerenciamento como apagamento remoto, dispositivos compartilhados ou afinidade de usuários em um dispositivo.

Os seguintes recursos do Graph estão disponíveis para gerenciar registros no Intune:  

- [Configuração de registro do dispositivo](intune-onboarding-deviceenrollmentconfiguration.md)
- [Configuração de limite do registro do dispositivo](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [Restrição da plataforma de registro do dispositivo](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [Configuração das restrições da plataforma de registro do dispositivo](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [Configuração do Windows Hello para empresas do registro do dispositivo](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [Conector do Exchange de gerenciamento de dispositivo](intune-onboarding-devicemanagementexchangeconnector.md)
- [Status de conector do exchange de gerenciamento de dispositivo](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [Tipo de sincronização de conector do exchange de gerenciamento de dispositivo](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [Tipo de conector do exchange de gerenciamento de dispositivo](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [Parceiro de gerenciamento do dispositivo](intune-onboarding-devicemanagementpartner.md)
- [Tipo de aplicativo de parceiro de gerenciamento de dispositivo](intune-onboarding-devicemanagementpartnerapptype.md)
- [Estado de locatário de parceiro de gerenciamento de dispositivo](intune-onboarding-devicemanagementpartnertenantstate.md)
- [Habilitação de](intune-onboarding-enablement.md)
- [Atribuição de configuração do registro](intune-onboarding-enrollmentconfigurationassignment.md)
- [Marca Intune](intune-onboarding-intunebrand.md)
- [Autoridade MDM](intune-onboarding-mdmauthority.md)
- [Conector de defesa contra ameaças móveis](intune-onboarding-mobilethreatdefenseconnector.md)
- [Estado de locatário de parceiro ameaças móveis](intune-onboarding-mobilethreatpartnertenantstate.md)
- [Configuração de acesso condicional local](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [Organização](intune-onboarding-organization.md)
- [Cores RGB](intune-onboarding-rgbcolor.md)
- [Token VPP](intune-onboarding-vpptoken.md)
- [Estado de token VPP](intune-onboarding-vpptokenstate.md)
- [Status da sincronização de token de VPP](intune-onboarding-vpptokensyncstatus.md)
- [Windows Olá para uso PIN de negócios](intune-onboarding-windowshelloforbusinesspinusage.md)
