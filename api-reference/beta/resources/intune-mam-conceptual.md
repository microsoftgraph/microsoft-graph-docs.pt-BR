---
title: Gerenciar aplicativos móveis com Microsoft Intune – Microsoft API do Graph
description: Lista o Microsoft API do Graph para Intune de extremidade (REST) relacionados ao MAM (gerenciamento de aplicativo móvel) para uma organização de locatários.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
ms.openlocfilehash: 97180d2dc1f317fbab1cf63e8414b77693605db1
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66667387"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a>Como proteger dados de aplicativos corporativos com o Microsoft Intune

Namespace: microsoft.graph

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

As políticas de proteção de aplicativos do Microsoft Intune ajudam a proteger os dados da empresa e evitar a perda de dados.

Use as políticas de proteção de aplicativos do Intune para ajudar a proteger os dados da sua empresa. Como Intune políticas de proteção de aplicativo podem ser usadas independentemente de qualquer solução de MDM (gerenciamento de dispositivo móvel), você pode usá-la para proteger os dados da sua empresa com ou sem registrar dispositivos em uma solução de gerenciamento de dispositivo. Implementando as políticas de nível de aplicativo, é possível restringir o acesso aos recursos da empresa e manter os dados dentro do âmbito do seu departamento de TI.

Os seguintes recursos do Graph estão disponíveis para gerenciar políticas de proteção de aplicativos no Intune:

- [Registro de aplicativo gerenciado Android](intune-mam-androidmanagedappregistration.md)
- [Tipo de verificação de aplicativos de rede de segurança em aplicativo gerenciado para Android](intune-mam-androidmanagedappsafetynetappsverificationtype.md)
- [Tipo de atestado de dispositivo de rede de segurança do aplicativo gerenciado para Android](intune-mam-androidmanagedappsafetynetdeviceattestationtype.md)
- [Tipo de avaliação da rede de segurança do aplicativo gerenciado android](intune-mam-androidmanagedappsafetynetevaluationtype.md)
- [Identificador de aplicativo móvel Android](intune-mam-androidmobileappidentifier.md)
- [Nível de gerenciamento de aplicativo](intune-mam-appmanagementlevel.md)
- [Tipo de aplicativo](intune-wip-applicationtype.md)
- [Proteção de aplicativo gerenciado padrão](intune-mam-defaultmanagedappprotection.md)
- [Aplicabilidade da configuração do Exchange Online de configuração de gerenciamento de dispositivos](intune-mam-devicemanagementconfigurationexchangeonlinesettingapplicability.md)
- [Aplicabilidade da definição de configuração de gerenciamento de dispositivos](intune-mam-devicemanagementconfigurationsettingapplicability.md)
- [Definição do valor da configuração da cadeia de caracteres de gerenciamento de dispositivo](intune-mam-devicemanagementconfigurationstringsettingvaluedefinition.md)
- [Tecnologias de configuração de gerenciamento de dispositivo](intune-mam-devicemanagementconfigurationtechnologies.md)
- [Aplicabilidade da configuração de configuração de gerenciamento de dispositivo](intune-mam-devicemanagementconfigurationwindowssettingapplicability.md)
- [Tipo de plataforma do dispositivo](intune-wip-deviceplatformtype.md)
- [Perfil de identidade visual do Intune](intune-wip-intunebrandingprofile.md)
- [Atribuição do perfil de identidade visual do Intune](intune-wip-intunebrandingprofileassignment.md)
- [Registro de aplicativo gerenciado iOS](intune-mam-iosmanagedappregistration.md)
- [Identificador de aplicativo móvel iOS](intune-mam-iosmobileappidentifier.md)
- [JSON](intune-mam-json.md)
- [Par chave/valor](intune-mam-keyvaluepair.md)
- [Identificador do aplicativo Mac](intune-mam-macappidentifier.md)
- [Nível de compartilhamento de área de transferência do aplicativo gerenciado](intune-mam-managedappclipboardsharinglevel.md)
- [Configuração de aplicativo gerenciado](intune-mam-managedappconfiguration.md)
- [Tipo de criptografia de dados do aplicativo gerenciado](intune-mam-managedappdataencryptiontype.md)
- [Local de ingestão de dados do aplicativo gerenciado](intune-mam-managedappdataingestionlocation.md)
- [Local de armazenamento de dados do aplicativo gerenciado](intune-mam-managedappdatastoragelocation.md)
- [Nível de transferência de dados do aplicativo gerenciado](intune-mam-managedappdatatransferlevel.md)
- [Nível de ameaça do dispositivo de aplicativo gerenciado](intune-mam-managedappdevicethreatlevel.md)
- [Status de diagnóstico de aplicativo gerenciado](intune-mam-managedappdiagnosticstatus.md)
- [Motivo de sinalização do aplicativo gerenciado](intune-mam-managedappflaggedreason.md)
- [Restrição de notificação de aplicativo gerenciado](intune-mam-managedappnotificationrestriction.md)
- [Operação de aplicativo gerenciado](intune-mam-managedappoperation.md)
- [Nível de redirecionamento de número de telefone do aplicativo gerenciado](intune-mam-managedappphonenumberredirectlevel.md)
- [Conjunto de caracteres do PIN do aplicativo gerenciado](intune-mam-managedapppincharacterset.md)
- [Política de aplicativo gerenciado](intune-mam-managedapppolicy.md)
- [Resumo da implantação da política de aplicativo gerenciado](intune-mam-managedapppolicydeploymentsummary.md)
- [Resumo por aplicativo da implantação da política de aplicativo gerenciado](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [Proteção de aplicativo gerenciado](intune-mam-managedappprotection.md)
- [Registro de aplicativo gerenciado](intune-mam-managedappregistration.md)
- [Ação de reparo do aplicativo gerenciado](intune-mam-managedappremediationaction.md)
- [Status de aplicativo gerenciado](intune-mam-managedappstatus.md)
- [Status bruto de aplicativo gerenciado](intune-mam-managedappstatusraw.md)
- [Tipo de navegador gerenciado](intune-mam-managedbrowsertype.md)
- [Aplicativo móvel gerenciado](intune-mam-managedmobileapp.md)
- [Identificador de aplicativo móvel](intune-mam-mobileappidentifier.md)
- [Tipo de grupo de aplicativos gerenciados direcionado](intune-mam-targetedmanagedappgrouptype.md)
- [Atribuição de política de proteção de aplicativo gerenciado direcionado](intune-mam-targetedmanagedapppolicyassignment.md)
- [Proteção de aplicativo gerenciado direcionado](intune-mam-targetedmanagedappprotection.md)
- [Identificador de aplicativo do Windows](intune-mam-windowsappidentifier.md)
- [Proteção de informações do Windows](intune-mam-windowsinformationprotection.md)
- [Arquivo de proteção de informações do Windows](intune-mam-windowsinformationprotectionapp.md)
- [Resumo de aprendizagem de aplicativos da proteção de informações do Windows](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [Arquivo do bloqueador de aplicativos da proteção de informações do Windows](intune-mam-windowsinformationprotectionapplockerfile.md)
- [Certificado de recuperação de dados de proteção de informações do Windows](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [Aplicativo da área de trabalho da proteção de informações do Windows](intune-mam-windowsinformationprotectiondesktopapp.md)
- [Registro de dispositivo de proteção de informações do Windows](intune-mam-windowsinformationprotectiondeviceregistration.md)
- [Nível de aplicação da proteção de informações do Windows](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [Coleção de intervalos de IP da Proteção de Informações do Windows](intune-mam-windowsinformationprotectioniprangecollection.md)
- [Resumo de aprendizagem da rede de proteção de informações do Windows](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [Requisitos de caracteres do PIN de proteção de informações do Windows](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [Política de proteção de informações do Windows](intune-mam-windowsinformationprotectionpolicy.md)
- [Coleção de domínios como proxy da Proteção de Informações do Windows](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [Coleção de recursos da Proteção de Informações do Windows](intune-mam-windowsinformationprotectionresourcecollection.md)
- [Aplicativo de loja de proteção de informações do Windows](intune-mam-windowsinformationprotectionstoreapp.md)
- [Ação wipe de proteção de informações do Windows](intune-mam-windowsinformationprotectionwipeaction.md)
- [Nível de compartilhamento da área de transferência de aplicativo gerenciado do Windows](intune-mam-windowsmanagedappclipboardsharinglevel.md)
- [Nível de transferência de dados do aplicativo gerenciado do Windows](intune-mam-windowsmanagedappdatatransferlevel.md)
- [Proteção de aplicativo gerenciado do Windows](intune-mam-windowsmanagedappprotection.md)
