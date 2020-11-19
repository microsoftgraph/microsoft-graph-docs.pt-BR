---
title: tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 282915b085107d5367a0b7f8bd8f4f3ea84b7c23
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49258938"
---
# <a name="managementagenttype-enum-type"></a>tipo de enumeração managementAgentType

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de agente de gerenciamento.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Estendi|1|O dispositivo é gerenciado pelo Exchange Server.|
|MDM|duas|O dispositivo é gerenciado pelo MDM do Intune.|
|easMdm|3D|O dispositivo é gerenciado pelo Exchange Server e o MDM do Intune.|
|intuneClient|4 |Cliente do Intune gerenciado.|
|easIntuneClient|5 |O dispositivo é ESTENDIdo e o cliente do Intune é gerenciado duas.|
|configurationManagerClient|8 |O dispositivo é gerenciado pelo Configuration Manager.|
|configurationManagerClientMdm|10 |O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.|
|configurationManagerClientMdmEas|11 |O dispositivo é gerenciado pelo Configuration Manager, MDM e EAS.|
|desconhecido|16 |Tipo de agente de gerenciamento desconhecido.|
|jamf|32|Os atributos do dispositivo são buscados do JAMF.|
|googleCloudDevicePolicyController|64|O dispositivo é gerenciado pelo CloudDPC do Google.|
|microsoft365ManagedMdm|258|Este dispositivo é gerenciado pelo Microsoft 365 por meio do Intune.|
|windowsManagementCloudApi|512|Este dispositivo é gerenciado pela API de nuvem de gerenciamento do Windows.|




