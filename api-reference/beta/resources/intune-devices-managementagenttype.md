---
title: tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb948626035bed2dac7ee18d103aa083bd0f2aeb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172538"
---
# <a name="managementagenttype-enum-type"></a>tipo de enumeração managementAgentType

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de agente de gerenciamento.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Estendi|1|O dispositivo é gerenciado pelo Exchange Server.|
|MDM|duas|O dispositivo é gerenciado pelo MDM do Intune.|
|easMdm|3D|O dispositivo é gerenciado pelo Exchange Server e o MDM do Intune.|
|intuneClient|quatro|Cliente do Intune gerenciado.|
|easIntuneClient|0,5|O dispositivo é ESTENDIdo e o cliente do Intune é gerenciado duas.|
|configurationManagerClient|8|O dispositivo é gerenciado pelo Configuration Manager.|
|configurationManagerClientMdm|254|O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.|
|configurationManagerClientMdmEas|11|O dispositivo é gerenciado pelo Configuration Manager, MDM e EAS.|
|unknown|dezesseis|Tipo de agente de gerenciamento desconhecido.|
|JAMF|32|Os atributos do dispositivo são buscados do JAMF.|
|googleCloudDevicePolicyController|64|O dispositivo é gerenciado pelo CloudDPC do Google.|
|microsoft365ManagedMdm|258|Este dispositivo é gerenciado pelo Microsoft 365 por meio do Intune.|




