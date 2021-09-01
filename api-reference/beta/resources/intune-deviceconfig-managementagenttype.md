---
title: tipo de número managementAgentType
description: Tipo de agente de gerenciamento.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 88670bf7bee32898bd18efea79153096c289cf5e
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789612"
---
# <a name="managementagenttype-enum-type"></a>tipo de número managementAgentType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de agente de gerenciamento.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|eas|1|O dispositivo é gerenciado por Exchange servidor.|
|mdm|2|O dispositivo é gerenciado pelo MDM do Intune.|
|easMdm|3|O dispositivo é gerenciado pelo servidor Exchange e pelo MDM do Intune.|
|intuneClient|4 |Cliente do Intune gerenciado.|
|easIntuneClient|5 |O dispositivo é gerenciado duplo do cliente EAS e do Intune.|
|configurationManagerClient|8 |O dispositivo é gerenciado pelo Configuration Manager.|
|configurationManagerClientMdm|10 |O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.|
|configurationManagerClientMdmEas|11 |O dispositivo é gerenciado pelo Configuration Manager, MDM e Eas.|
|desconhecido|16 |Tipo de agente de gerenciamento desconhecido.|
|jamf|32|Os atributos do dispositivo são buscados do Jamf.|
|googleCloudDevicePolicyController|64|O dispositivo é gerenciado pelo CloudDPC do Google.|
|microsoft365ManagedMdm|258|Esse dispositivo é gerenciado por Microsoft 365 através do Intune.|
|windowsManagementCloudApi|512|Esse dispositivo é gerenciado pela API de Nuvem de Gerenciamento Windows Gerenciamento.|



