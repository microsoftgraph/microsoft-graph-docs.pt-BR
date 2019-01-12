---
title: Registrar dispositivos de propriedade corporativa por meio do Intune
description: " Cenário de (BYOD)."
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9671eb7f66be78075209906a4f6f923256afef36
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928021"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a>Registrar dispositivos de propriedade corporativa por meio do Intune

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.

É possível registrar dispositivos pertencentes à organização ou de propriedade corporativa para serem gerenciados com o Intune de várias maneiras, dependendo do tipo de dispositivo, de como o dispositivo foi comprado e das necessidades da organização. Também é possível instalar o aplicativo Portal da Empresa para registrar e gerenciar dispositivos de propriedade corporativa, como em um cenário "traga seu próprio dispositivo" (BYOD).

Os seguintes recursos do Graph estão disponíveis para gerenciar dispositivos corporativos no Intune:

- [Perfil de implantação de piloto automático do windows do Active directory](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [Perfil de implantação piloto automático do Azure AD windows](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [Perfil básico do DEP inscrição](intune-enrollment-depenrollmentbaseprofile.md)
- [Perfil de inscrição do DEP](intune-enrollment-depenrollmentprofile.md)
- [Perfil de inscrição do DEP iOS](intune-enrollment-depiosenrollmentprofile.md)
- [Perfil de inscrição do DEP macOS](intune-enrollment-depmacosenrollmentprofile.md)
- [Configuração de nível de contratação DEP](intune-enrollment-deponboardingsetting.md)
- [Tipo de token de DEP](intune-enrollment-deptokentype.md)
- [Origem de descoberta](intune-enrollment-discoverysource.md)
- [Perfil de inscrição](intune-enrollment-enrollmentprofile.md)
- [Estado de inscrição](intune-enrollment-enrollmentstate.md)
- [Identidade de dispositivo importada Apple](intune-enrollment-importedappledeviceidentity.md)
- [Importado resultado de identidade do dispositivo Apple](intune-enrollment-importedappledeviceidentityresult.md)
- [Identidade do dispositivo importada](intune-enrollment-importeddeviceidentity.md)
- [Importado resultado de identidade do dispositivo](intune-enrollment-importeddeviceidentityresult.md)
- [Tipo de identidade do dispositivo de importado](intune-enrollment-importeddeviceidentitytype.md)
- [Identidade de dispositivo do windows importados piloto automático](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [Status de importação de identidade do windows importados piloto automático dispositivo](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [Estado de identidade do dispositivo do windows importados piloto automático](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [Carregamento de identidade do windows importados piloto automático dispositivo](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [Status de carregamento de identidade do dispositivo de piloto automático importados do windows](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [modo de emparelhamento iTunes](intune-enrollment-itunespairingmode.md)
- [Certificado com impressão digital de gerenciamento](intune-enrollment-managementcertificatewiththumbprint.md)
- [Configuração inicial pelo usuário configurações](intune-enrollment-outofboxexperiencesettings.md)
- [Plataforma](intune-enrollment-platform.md)
- [Perfil de implantação de piloto automático do Windows](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [Atribuição de perfil de implantação do Windows piloto automático](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [Identidade do dispositivo do Windows piloto automático](intune-enrollment-windowsautopilotdeviceidentity.md)
- [Atribuição de perfil de piloto automático do Windows detalhadas de status](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [Status de atribuição de perfil de piloto automático do Windows](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [Configurações de piloto automático do Windows](intune-enrollment-windowsautopilotsettings.md)
- [Status de sincronização do Windows piloto automático](intune-enrollment-windowsautopilotsyncstatus.md)
- [Tipo de uso de dispositivo do Windows](intune-enrollment-windowsdeviceusagetype.md)
- [Configurações de tela de status de registro do Windows](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [Tipo de usuário do Windows](intune-enrollment-windowsusertype.md)
