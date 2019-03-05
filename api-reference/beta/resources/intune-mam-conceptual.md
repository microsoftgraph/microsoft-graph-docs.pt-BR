---
title: Gerenciar aplicativos móveis com o Microsoft Intune-API do Microsoft Graph
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) relacionadas ao gerenciamento de aplicativo móvel (MAM) para uma organização de locatário.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4443c78c6ae58979b0390496d8d560bb15a90669
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150397"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a>Como proteger dados de aplicativos corporativos com o Microsoft Intune

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.

As políticas de proteção de aplicativos do Microsoft Intune ajudam a proteger os dados da empresa e evitar a perda de dados.

Use as políticas de proteção de aplicativos do Intune para ajudar a proteger os dados da sua empresa. Como as políticas de proteção de aplicativos do Intune podem ser usadas independentemente de qualquer solução de gerenciamento de dispositivo móvel (MDM), você pode usá-la para proteger os dados da sua empresa com ou sem o registro de dispositivos em uma solução de gerenciamento de dispositivo. Implementando as políticas de nível de aplicativo, é possível restringir o acesso aos recursos da empresa e manter os dados dentro do âmbito do seu departamento de TI.

Os seguintes recursos do Graph estão disponíveis para gerenciar políticas de proteção de aplicativos no Intune:

- [Proteção de aplicativo gerenciado Android](intune-mam-androidmanagedappprotection.md)
- [Registro de aplicativo gerenciado Android](intune-mam-androidmanagedappregistration.md)
- [Identificador de aplicativo móvel Android](intune-mam-androidmobileappidentifier.md)
- [Nível de gerenciamento de aplicativo](intune-mam-appmanagementlevel.md)
- [Tipo de aplicativo](intune-wip-applicationtype.md)
- [Proteção de aplicativo gerenciado padrão](intune-mam-defaultmanagedappprotection.md)
- [Perfil de identidade visual do Intune](intune-wip-intunebrandingprofile.md)
- [Atribuição do perfil de identidade visual do Intune](intune-wip-intunebrandingprofileassignment.md)
- [Proteção de aplicativo gerenciado iOS](intune-mam-iosmanagedappprotection.md)
- [Registro de aplicativo gerenciado iOS](intune-mam-iosmanagedappregistration.md)
- [Identificador de aplicativo móvel iOS](intune-mam-iosmobileappidentifier.md)
- [JSON](intune-mam-json.md)
- [Nível de compartilhamento de área de transferência do aplicativo gerenciado](intune-mam-managedappclipboardsharinglevel.md)
- [Configuração de aplicativo gerenciado](intune-mam-managedappconfiguration.md)
- [Tipo de criptografia de dados do aplicativo gerenciado](intune-mam-managedappdataencryptiontype.md)
- [Local de armazenamento de dados do aplicativo gerenciado](intune-mam-managedappdatastoragelocation.md)
- [Nível de transferência de dados do aplicativo gerenciado](intune-mam-managedappdatatransferlevel.md)
- [Status de diagnóstico de aplicativo gerenciado](intune-mam-managedappdiagnosticstatus.md)
- [Motivo de sinalização do aplicativo gerenciado](intune-mam-managedappflaggedreason.md)
- [Operação de aplicativo gerenciado](intune-mam-managedappoperation.md)
- [Conjunto de caracteres do PIN do aplicativo gerenciado](intune-mam-managedapppincharacterset.md)
- [Política de aplicativo gerenciado](intune-mam-managedapppolicy.md)
- [Resumo da implantação da política de aplicativo gerenciado](intune-mam-managedapppolicydeploymentsummary.md)
- [Resumo por aplicativo da implantação da política de aplicativo gerenciado](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [Proteção de aplicativo gerenciado](intune-mam-managedappprotection.md)
- [Registro de aplicativo gerenciado](intune-mam-managedappregistration.md)
- [Ação de reparo do aplicativo gerenciado](intune-mam-managedappremediationaction.md)
- [Status de aplicativo gerenciado](intune-mam-managedappstatus.md)
- [Status bruto de aplicativo gerenciado](intune-mam-managedappstatusraw.md)
- [Aplicativo móvel gerenciado](intune-mam-managedmobileapp.md)
- [Política de proteção de informações do Windows MDM](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [Identificador de aplicativo móvel](intune-mam-mobileappidentifier.md)
- [Configuração direcionada de aplicativo gerenciado](intune-mam-targetedmanagedappconfiguration.md)
- [Atribuição de política de proteção de aplicativo gerenciado direcionado](intune-mam-targetedmanagedapppolicyassignment.md)
- [Proteção de aplicativo gerenciado direcionado](intune-mam-targetedmanagedappprotection.md)
- [Proteção de informações do Windows](intune-mam-windowsinformationprotection.md)
- [Arquivo de proteção de informações do Windows](intune-mam-windowsinformationprotectionapp.md)
- [Resumo de aprendizagem de aplicativos da proteção de informações do Windows](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [Arquivo do bloqueador de aplicativos da proteção de informações do Windows](intune-mam-windowsinformationprotectionapplockerfile.md)
- [Certificado de recuperação de dados de proteção de informações do Windows](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [Aplicativo da área de trabalho da proteção de informações do Windows](intune-mam-windowsinformationprotectiondesktopapp.md)
- [Registro de dispositivo de proteção de informações do Windows](intune-mam-windowsinformationprotectiondeviceregistration.md)
- [Nível de aplicação da ´proteção de informações do Windows](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [Coleção de intervalos de IP da Proteção de Informações do Windows](intune-mam-windowsinformationprotectioniprangecollection.md)
- [Resumo de aprendizagem da rede de proteção de informações do Windows](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [Requisitos de caracteres do PIN de proteção de informações do Windows](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [Política de proteção de informações do Windows](intune-mam-windowsinformationprotectionpolicy.md)
- [Coleção de domínios como proxy da Proteção de Informações do Windows](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [Coleção de recursos da Proteção de Informações do Windows](intune-mam-windowsinformationprotectionresourcecollection.md)
- [Aplicativo de loja de proteção de informações do Windows](intune-mam-windowsinformationprotectionstoreapp.md)
- [Ação wipe de proteção de informações do Windows](intune-mam-windowsinformationprotectionwipeaction.md)
