---
title: Recursos compartilhados em Microsoft Intune - API Graph Microsoft
description: Lista a API Graph microsoft para pontos de extremidade do Intune (REST) que suportam vários fluxos de trabalho para uma organização de locatários.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 9ef71ce51e86d2582935a5f647a0a7ad07b70e73
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58264077"
---
# <a name="shared-resources-in-microsoft-intune"></a>Recursos compartilhados em Microsoft Intune

Namespace: microsoft.graph

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Esses pontos de extremidade são usados em várias API do Microsoft Graph para fluxos de trabalho do Intune.  A intenção, a finalidade e as permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.  Além disso, determinados métodos, propriedades e ações são suportados apenas para fluxos de trabalho específicos.

Os seguintes Graph são compartilhados entre fluxos de trabalho do Intune:

- [Estado da ação](intune-shared-actionstate.md)
- [Destino de atribuição de todos os dispositivos](intune-shared-alldevicesassignmenttarget.md)
- [Destino de atribuição de todos os usuários licenciados](intune-shared-alllicensedusersassignmenttarget.md)
- [Android enterprise sempre no tipo de pacote VPN](intune-shared-androidenterprisealwaysonvpnpackagetype.md)
- [Proteção de aplicativo gerenciado Android](intune-shared-androidmanagedappprotection.md)
- [Configurações de atribuição de aplicativo de loja gerenciada do Android](intune-shared-androidmanagedstoreappassignmentsettings.md)
- [Armazenamento de destino de certificados](intune-shared-certificatedestinationstore.md)
- [Repositório de certificados](intune-shared-certificatestore.md)
- [Escala de período de validade do certificado](intune-shared-certificatevalidityperiodscale.md)
- [Ação do portal da empresa](intune-shared-companyportalaction.md)
- [Ação bloqueada do portal da empresa](intune-shared-companyportalblockedaction.md)
- [Status de conformidade](intune-shared-compliancestatus.md)
- [Destino da atribuição da coleção configuration manager](intune-shared-configurationmanagercollectionassignmenttarget.md)
- [Tipo de filtro de atribuição de gerenciamento de dispositivos e aplicativos](intune-shared-deviceandappmanagementassignmentfiltertype.md)
- [Fonte de atribuição de gerenciamento de dispositivos e aplicativos](intune-shared-deviceandappmanagementassignmentsource.md)
- [Destino de atribuição de gerenciamento de aplicativo e dispositivo](intune-shared-deviceandappmanagementassignmenttarget.md)
- [Gerenciamento de aplicativos de dispositivo](intune-shared-deviceappmanagement.md)
- [Categoria do dispositivo](intune-shared-devicecategory.md)
- [Política de conformidade do dispositivo](intune-shared-devicecompliancepolicy.md)
- [Configuração do dispositivo](intune-shared-deviceconfiguration.md)
- [Configuração de registro do dispositivo](intune-shared-deviceenrollmentconfiguration.md)
- [Gerenciamento de dispositivo](intune-shared-devicemanagement.md)
- [Configurações de credenciais derivadas do gerenciamento de dispositivos](intune-shared-devicemanagementderivedcredentialsettings.md)
- [Script de gerenciamento de dispositivo](intune-shared-devicemanagementscript.md)
- [Habilitação](intune-shared-enablement.md)
- [Opções de disponibilidade de registro](intune-shared-enrollmentavailabilityoptions.md)
- [Estado de registro](intune-shared-enrollmentstate.md)
- [Destino de atribuição de grupos de exclusão](intune-shared-exclusiongroupassignmenttarget.md)
- [Uso estendido de chave](intune-shared-extendedkeyusage.md)
- [Destino de atribuição de grupo](intune-shared-groupassignmenttarget.md)
- [Algoritmos hash](intune-shared-hashalgorithms.md)
- [Intenção de instalação](intune-shared-installintent.md)
- [Configurações de atribuição do aplicativo LOB do iOS](intune-shared-ioslobappassignmentsettings.md)
- [Configuração de provisionamento do aplicativo LOB do iOS](intune-shared-ioslobappprovisioningconfiguration.md)
- [Proteção de aplicativo gerenciado iOS](intune-shared-iosmanagedappprotection.md)
- [Configurações de atribuição de aplicativo da loja iOS](intune-shared-iosstoreappassignmentsettings.md)
- [Configurações de atribuição do aplicativo VPP do iOS](intune-shared-iosvppappassignmentsettings.md)
- [Intervalo de IP](intune-shared-iprange.md)
- [Intervalo de IPv4](intune-shared-ipv4range.md)
- [Intervalo de IPv6](intune-shared-ipv6range.md)
- [Tamanho da chave](intune-shared-keysize.md)
- [Opção de provedor de armazenamento de chaves](intune-shared-keystorageprovideroption.md)
- [Usos de chave](intune-shared-keyusages.md)
- [Configurações de atribuição do aplicativo LOB do macOS](intune-shared-macoslobappassignmentsettings.md)
- [Configurações de atribuição do aplicativo VPP do macOS](intune-shared-macosvppappassignmentsettings.md)
- [Tipo de proprietário do dispositivo gerenciado](intune-shared-manageddeviceownertype.md)
- [Política de proteção de informações do Windows MDM](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [Configurações de atribuição do aplicativo da Microsoft Store para Empresas](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [Conteúdo MIME](intune-shared-mimecontent.md)
- [Aplicativo móvel](intune-shared-mobileapp.md)
- [Configurações de atribuição de aplicativo móvel](intune-shared-mobileappassignmentsettings.md)
- [Configurações de tempo de instalação do aplicativo móvel](intune-shared-mobileappinstalltimesettings.md)
- [Evento de solução de problemas de aplicativo móvel](intune-shared-mobileapptroubleshootingevent.md)
- [Tipo de proprietário](intune-shared-ownertype.md)
- [Domínio com proxy](intune-shared-proxieddomain.md)
- [Report](intune-shared-report.md)
- [Raiz de relatório](intune-shared-reportroot.md)
- [Cores RGB](intune-shared-rgbcolor.md)
- [Executar como tipo de conta](intune-shared-runasaccounttype.md)
- [Opções de geração do estado da interface do usuário salvas](intune-shared-saveduistategenerationoptions.md)
- [Definindo o tipo de origem](intune-shared-settingsourcetype.md)
- [Tipo de nome alternativo da entidade](intune-shared-subjectalternativenametype.md)
- [Configuração direcionada de aplicativo gerenciado](intune-shared-targetedmanagedappconfiguration.md)
- [URI](intune-shared-uri.md)
- [Usuário](intune-shared-user.md)
- [Tipo de conta do token VPP](intune-shared-vpptokenaccounttype.md)
- [Causa da falha da ação do token VPP](intune-shared-vpptokenactionfailurereason.md)
- [Configurações de atribuição do aplicativo LOB do Win32](intune-shared-win32lobappassignmentsettings.md)
- [Prioridade de otimização de entrega de aplicativos LOB win32](intune-shared-win32lobappdeliveryoptimizationpriority.md)
- [Notificação de aplicativo LOB do Win32](intune-shared-win32lobappnotification.md)
- [Configurações de reinicialização do aplicativo LOB do Win32](intune-shared-win32lobapprestartsettings.md)
- [Configurações de atribuição do aplicativo Windows AppX](intune-shared-windowsappxappassignmentsettings.md)
- [Perfil de implantação do Windows Autopilot](intune-shared-windowsautopilotdeploymentprofile.md)
- [Configuração de ingresso no domínio do Windows](intune-shared-windowsdomainjoinconfiguration.md)
- [Configurações de atribuição do aplicativo Windows universal AppX](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [Windows estado de atualização](intune-shared-windowsupdatestate.md)