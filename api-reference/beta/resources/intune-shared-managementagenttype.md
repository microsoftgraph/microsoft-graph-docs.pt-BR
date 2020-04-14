---
title: tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 34783f2c586e192d62cdeb0018b82e2df100c958
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466240"
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
|configurationManagerClientMdmEas|11|O dispositivo é gerenciado pelo Configuration Manager, MDM e EAS.|
|desconhecido|16 |Tipo de agente de gerenciamento desconhecido.|
|jamf|32|Os atributos do dispositivo são buscados do JAMF.|
|googleCloudDevicePolicyController|64|O dispositivo é gerenciado pelo CloudDPC do Google.|
|microsoft365ManagedMdm|258|Este dispositivo é gerenciado pelo Microsoft 365 por meio do Intune.|
|windowsManagementCloudApi|512|Este dispositivo é gerenciado pela API de nuvem de gerenciamento do Windows.|



