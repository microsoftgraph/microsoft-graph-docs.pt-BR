---
title: Registrar dispositivos para o gerenciamento no Intune
description: " O registro (BYOD) permite que os usuários inscrevam seus telefones pessoais, tablets ou computadores. O registro de dispositivo de propriedade corporativa (COD) permite cenários de gerenciamento como apagamento remoto, dispositivos compartilhados ou afinidade de usuários em um dispositivo."
ms.localizationpriority: medium
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 7e435246df7b2f57ab5f7d18d90ada3c56ec6579
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098668"
---
# <a name="enroll-devices-for-management-in-intune"></a>Registrar dispositivos para o gerenciamento no Intune

Namespace: microsoft.graph

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.

É possível registrar dispositivos, incluindo computadores Windows, para habilitar o gerenciamento de dispositivo móvel (MDM) com o Microsoft Intune. Este tópico descreve as diferentes maneiras de registrar dispositivos móveis no gerenciamento do Intune. A maneira de registrar dispositivos depende do tipo de dispositivo, da propriedade e do nível de gerenciamento necessário. O registro "Traga seu próprio dispositivo" (BYOD) permite aos usuários registrar seus telefones, computador e tablets pessoais. O registro de dispositivo de propriedade corporativa (COD) permite cenários de gerenciamento como apagamento remoto, dispositivos compartilhados ou afinidade de usuários em um dispositivo.

Os seguintes recursos do Graph estão disponíveis para gerenciar registros no Intune:  

- [Parceiro de gerenciamento de conformidade](intune-onboarding-compliancemanagementpartner.md)
- [Atribuição de parceiro de gerenciamento de conformidade](intune-onboarding-compliancemanagementpartnerassignment.md)
- [Gerenciamento de aplicativos de dispositivo](intune-onboarding-deviceappmanagement.md)
- [Categoria do dispositivo](intune-onboarding-devicecategory.md)
- [Configuração de registro do dispositivo](intune-onboarding-deviceenrollmentconfiguration.md)
- [Configuração de limite do registro do dispositivo](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [Restrição da plataforma de registro do dispositivo](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [Configuração das restrições da plataforma de registro do dispositivo](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [Configuração do Windows Hello para empresas do registro do dispositivo](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [Gerenciamento de dispositivo](intune-onboarding-devicemanagement.md)
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
- [Usuário](intune-onboarding-user.md)
- [Token VPP](intune-onboarding-vpptoken.md)
- [Estado do token VPP](intune-onboarding-vpptokenstate.md)
- [Status de sincronização do token VPP](intune-onboarding-vpptokensyncstatus.md)
- [Uso do PIN do Windows Hello para empresas](intune-onboarding-windowshelloforbusinesspinusage.md)
