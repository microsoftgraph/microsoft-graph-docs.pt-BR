---
title: Registrar dispositivos corporativos usando o Intune-Microsoft Graph API
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) que registram dispositivos para uma organização de locatário.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: f784f3aa837f13f009bd7520e89e045f8d952292
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999308"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a>Registrar dispositivos de propriedade corporativa por meio do Intune

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

É possível registrar dispositivos pertencentes à organização ou de propriedade corporativa para serem gerenciados com o Intune de várias maneiras, dependendo do tipo de dispositivo, de como o dispositivo foi comprado e das necessidades da organização. Também é possível instalar o aplicativo Portal da Empresa para registrar e gerenciar dispositivos de propriedade corporativa, como em um cenário "traga seu próprio dispositivo" (BYOD).

Os seguintes recursos do Graph estão disponíveis para gerenciar dispositivos corporativos no Intune:

- [Perfil de implantação do Windows Autopilot do Active Directory](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [Perfil de implantação do Windows Autopilot do Azure AD](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [Perfil básico de registro do DEP](intune-enrollment-depenrollmentbaseprofile.md)
- [Perfil de registro do DEP](intune-enrollment-depenrollmentprofile.md)
- [Perfil de registro de iOS do DEP](intune-enrollment-depiosenrollmentprofile.md)
- [Perfil de registro de macOS do DEP](intune-enrollment-depmacosenrollmentprofile.md)
- [Configuração de integração do DEP](intune-enrollment-deponboardingsetting.md)
- [Tipo de token do DEP](intune-enrollment-deptokentype.md)
- [Fonte de descoberta](intune-enrollment-discoverysource.md)
- [Perfil de registro](intune-enrollment-enrollmentprofile.md)
- [Estado de registro](intune-enrollment-enrollmentstate.md)
- [Identidade do dispositivo Apple importada](intune-enrollment-importedappledeviceidentity.md)
- [Importar resultado de identidade do dispositivo Apple](intune-enrollment-importedappledeviceidentityresult.md)
- [Identidade do dispositivo importada](intune-enrollment-importeddeviceidentity.md)
- [Resultado de identidade do dispositivo importada](intune-enrollment-importeddeviceidentityresult.md)
- [Tipo de identidade do dispositivo importada](intune-enrollment-importeddeviceidentitytype.md)
- [Identidade importada do dispositivo do Windows autopilot](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [Status de importação da identidade de dispositivo importada do windows autopilot](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [Estado de identidade de dispositivo importado do windows autopilot](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [Carregar identidade de dispositivo importado do windows autopilot](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [Status de carregamento da identidade de dispositivo importado do windows autopilot](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [Modo de emparelhamento do iTunes](intune-enrollment-itunespairingmode.md)
- [Certificado de gerenciamento com impressão digital](intune-enrollment-managementcertificatewiththumbprint.md)
- [Configurações de experiência iniciais](intune-enrollment-outofboxexperiencesettings.md)
- [Plataforma](intune-enrollment-platform.md)
- [Perfil de implantação do Windows Autopilot](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [Atribuição do perfil de implantação do Windows Autopilot](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [Identidade do dispositivo do Windows Autopilot](intune-enrollment-windowsautopilotdeviceidentity.md)
- [Tipo de dispositivo do Windows Autopilot](intune-enrollment-windowsautopilotdevicetype.md)
- [Status detalhado de atribuição do perfil do Windows Autopilot](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [Status de atribuição do perfil do Windows Autopilot](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [Configurações do Windows Autopilot](intune-enrollment-windowsautopilotsettings.md)
- [Status de sincronização do Windows Autopilot](intune-enrollment-windowsautopilotsyncstatus.md)
- [Tipo de uso do dispositivo Windows](intune-enrollment-windowsdeviceusagetype.md)
- [Configurações de tela de status de registro do Windows](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [Tipo de usuário do Windows](intune-enrollment-windowsusertype.md)
