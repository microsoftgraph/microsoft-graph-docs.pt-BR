---
title: tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9743c9c83e34a0c58dee78e73839f8fdcaaf2cda
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251563"
---
# <a name="managementagenttype-enum-type"></a>tipo de enumeração managementAgentType

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



