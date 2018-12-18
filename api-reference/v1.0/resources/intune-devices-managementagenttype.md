---
title: tipo de enum managementAgentType
description: Tipo de agente de gerenciamento.
author: tfitzmac
ms.openlocfilehash: b1f6db6eaea1a488831bec3d7ff61d6170414956
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355514"
---
# <a name="managementagenttype-enum-type"></a>tipo de enum managementAgentType

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Tipo de agente de gerenciamento.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|EAs|1|O dispositivo é gerenciado pelo Exchange server.|
|MDM|2|O dispositivo é gerenciado pelo MDM. Intune|
|easMdm|3|O dispositivo é gerenciado pelo Exchange server e MDM de Intune.|
|intuneClient|4|Cliente Intune gerenciados.|
|easIntuneClient|5|O dispositivo está EAS Intune cliente e dual gerenciado.|
|configurationManagerClient|8|O dispositivo é gerenciado pelo Gerenciador de configuração.|
|configurationManagerClientMdm|10|O dispositivo é gerenciado pelo Gerenciador de configuração e MDM.|
|configurationManagerClientMdmEas|11|O dispositivo é gerenciado pelo Gerenciador de configuração, MDM e Eas.|
|unknown|16|Tipo de agente de gerenciamento desconhecido.|
|jamf|32|Os atributos de dispositivo são buscados no Jamf.|
|googleCloudDevicePolicyController|64|O dispositivo é gerenciado por CloudDPC do Google.|



