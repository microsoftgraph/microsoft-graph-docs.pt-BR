---
title: tipo de enum automaticUpdateMode
description: Valores possíveis para o modo de atualização automática.
ms.openlocfilehash: b7eac8337d6c8286e538bbe98b5ecbc13a448628
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038917"
---
# <a name="automaticupdatemode-enum-type"></a>tipo de enum automaticUpdateMode

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis para o modo de atualização automática.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|Definido pelo usuário, valor padrão, sem intenção.|
|notifyDownload|1|Notifica baixados.|
|autoInstallAtMaintenanceTime|2|Instalar automaticamente em tempo de manutenção.|
|autoInstallAndRebootAtMaintenanceTime|3|Instalar automaticamente e reinicialize em tempo de manutenção.|
|autoInstallAndRebootAtScheduledTime|4|Instalar automaticamente e reinicialize no horário agendado.|
|autoInstallAndRebootWithoutEndUserControl|5|Instalar automaticamente e reinicie sem controle de usuário final|





