---
title: Gerenciar aplicativos móveis com Microsoft Intune - API Graph Microsoft
description: Lista a API Graph microsoft para pontos de extremidade do Intune (REST) relacionadas ao gerenciamento de aplicativos móveis (MAM) para uma organização de locatários.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
ms.openlocfilehash: d71c275d6b40e5c71f2f7ca737c93f99480b71d1
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61336157"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a>Como proteger dados de aplicativos corporativos com o Microsoft Intune

Namespace: microsoft.graph

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

As políticas de proteção de aplicativos do Microsoft Intune ajudam a proteger os dados da empresa e evitar a perda de dados.

Use as políticas de proteção de aplicativos do Intune para ajudar a proteger os dados da sua empresa. Como as políticas de proteção de aplicativos do Intune podem ser usadas independentemente de qualquer solução de gerenciamento de dispositivo móvel (MDM), você pode usá-los para proteger os dados da sua empresa com ou sem registrar dispositivos em uma solução de gerenciamento de dispositivos. Implementando as políticas de nível de aplicativo, é possível restringir o acesso aos recursos da empresa e manter os dados dentro do âmbito do seu departamento de TI.

Os seguintes recursos do Graph estão disponíveis para gerenciar políticas de proteção de aplicativos no Intune:

- [Registro de aplicativo gerenciado Android](intune-mam-androidmanagedappregistration.md)
- [Tipo de verificação de aplicativos de rede de segurança em aplicativo gerenciado para Android](intune-mam-androidmanagedappsafetynetappsverificationtype.md)
- [Tipo de atestado de dispositivo de rede de segurança do aplicativo gerenciado para Android](intune-mam-androidmanagedappsafetynetdeviceattestationtype.md)
- [Tipo de avaliação da rede de segurança de aplicativos gerenciados do Android](intune-mam-androidmanagedappsafetynetevaluationtype.md)
- [Identificador de aplicativo móvel Android](intune-mam-androidmobileappidentifier.md)
- [Nível de gerenciamento de aplicativo](intune-mam-appmanagementlevel.md)
- [Tipo de aplicativo](intune-wip-applicationtype.md)
- [Proteção de aplicativo gerenciado padrão](intune-mam-defaultmanagedappprotection.md)
- [Tipo de plataforma do dispositivo](intune-wip-deviceplatformtype.md)
- [Perfil de identidade visual do Intune](intune-wip-intunebrandingprofile.md)
- [Atribuição do perfil de identidade visual do Intune](intune-wip-intunebrandingprofileassignment.md)
- [Registro de aplicativo gerenciado iOS](intune-mam-iosmanagedappregistration.md)
- [Identificador de aplicativo móvel iOS](intune-mam-iosmobileappidentifier.md)
- [JSON](intune-mam-json.md)
- [Identificador de aplicativo Mac](intune-mam-macappidentifier.md)
- [Nível de compartilhamento de área de transferência do aplicativo gerenciado](intune-mam-managedappclipboardsharinglevel.md)
- [Configuração de aplicativo gerenciado](intune-mam-managedappconfiguration.md)
- [Tipo de criptografia de dados do aplicativo gerenciado](intune-mam-managedappdataencryptiontype.md)
- [Local de ingestão de dados do aplicativo gerenciado](intune-mam-managedappdataingestionlocation.md)
- [Local de armazenamento de dados do aplicativo gerenciado](intune-mam-managedappdatastoragelocation.md)
- [Nível de transferência de dados do aplicativo gerenciado](intune-mam-managedappdatatransferlevel.md)
- [Nível de ameaça de dispositivo de aplicativo gerenciado](intune-mam-managedappdevicethreatlevel.md)
- [Status de diagnóstico de aplicativo gerenciado](intune-mam-managedappdiagnosticstatus.md)
- [Motivo de sinalização do aplicativo gerenciado](intune-mam-managedappflaggedreason.md)
- [Restrição de notificação de aplicativo gerenciado](intune-mam-managedappnotificationrestriction.md)
- [Operação de aplicativo gerenciado](intune-mam-managedappoperation.md)
- [Nível de redirecionamento de número de telefone de aplicativo gerenciado](intune-mam-managedappphonenumberredirectlevel.md)
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
- [Tipo de grupo de aplicativo gerenciado direcionado](intune-mam-targetedmanagedappgrouptype.md)
- [Atribuição de política de proteção de aplicativo gerenciado direcionado](intune-mam-targetedmanagedapppolicyassignment.md)
- [Proteção de aplicativo gerenciado direcionado](intune-mam-targetedmanagedappprotection.md)
- [Windows de aplicativo](intune-mam-windowsappidentifier.md)
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
