---
title: Registrar dispositivos corporativos usando o Intune-Microsoft Graph API
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) que registram dispositivos para uma organização de locatário.
author: dougeby
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e8e1a03f5194b5790ba68c10dad8eae23a706945
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735236"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a>Registrar dispositivos de propriedade corporativa por meio do Intune

Namespace: microsoft.graph

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

É possível registrar dispositivos pertencentes à organização ou de propriedade corporativa para serem gerenciados com o Intune de várias maneiras, dependendo do tipo de dispositivo, de como o dispositivo foi comprado e das necessidades da organização. Também é possível instalar o aplicativo Portal da Empresa para registrar e gerenciar dispositivos de propriedade corporativa, como em um cenário "traga seu próprio dispositivo" (BYOD).

Os seguintes recursos do Graph estão disponíveis para gerenciar dispositivos corporativos no Intune:

- [Perfil de implantação do Windows Autopilot do Active Directory](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [Atribuição de perfil de registro da Apple](intune-enrollment-appleenrollmentprofileassignment.md)
- [Tipo de registro de tipo de proprietário da Apple](intune-enrollment-appleownertypeenrollmenttype.md)
- [Perfil de registro iniciado pelo usuário da Apple](intune-enrollment-appleuserinitiatedenrollmentprofile.md)
- [Tipo de registro iniciado pelo usuário da Apple](intune-enrollment-appleuserinitiatedenrollmenttype.md)
- [Perfil de implantação do Windows Autopilot do Azure AD](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [Perfil básico de registro do DEP](intune-enrollment-depenrollmentbaseprofile.md)
- [Perfil de registro do DEP](intune-enrollment-depenrollmentprofile.md)
- [Perfil de registro de iOS do DEP](intune-enrollment-depiosenrollmentprofile.md)
- [Perfil de registro de macOS do DEP](intune-enrollment-depmacosenrollmentprofile.md)
- [Configuração de integração do DEP](intune-enrollment-deponboardingsetting.md)
- [Tipo de token do DEP](intune-enrollment-deptokentype.md)
- [Fonte de descoberta](intune-enrollment-discoverysource.md)
- [Perfil de registro](intune-enrollment-enrollmentprofile.md)
- [Identidade do dispositivo Apple importada](intune-enrollment-importedappledeviceidentity.md)
- [Importar resultado de identidade do dispositivo Apple](intune-enrollment-importedappledeviceidentityresult.md)
- [Identidade do dispositivo importada](intune-enrollment-importeddeviceidentity.md)
- [Resultado de identidade do dispositivo importada](intune-enrollment-importeddeviceidentityresult.md)
- [Tipo de identidade do dispositivo importada](intune-enrollment-importeddeviceidentitytype.md)
- [Identidade importada do dispositivo do Windows autopilot](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [Status de importação da identidade de dispositivo importada do windows autopilot](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [Estado de identidade de dispositivo importado do windows autopilot](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [Status de carregamento da identidade de dispositivo importado do windows autopilot](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [Modo de emparelhamento do iTunes](intune-enrollment-itunespairingmode.md)
- [Certificado de gerenciamento com impressão digital](intune-enrollment-managementcertificatewiththumbprint.md)
- [Configurações de experiência iniciais](intune-enrollment-outofboxexperiencesettings.md)
- [Plataforma](intune-enrollment-platform.md)
- [Limite de registro sugerido](intune-enrollment-suggestedenrollmentlimit.md)
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