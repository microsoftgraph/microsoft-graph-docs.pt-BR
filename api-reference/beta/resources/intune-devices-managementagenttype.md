---
title: tipo de enum managementAgentType
description: Tipo de agente de gerenciamento.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9c42d4ea4a5114bc42966891e4cd60ea87ca303e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401002"
---
# <a name="managementagenttype-enum-type"></a>tipo de enum managementAgentType

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

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
|microsoft365ManagedMdm|258|Este dispositivo é gerenciado pelo Microsoft 365 através de Intune.|




