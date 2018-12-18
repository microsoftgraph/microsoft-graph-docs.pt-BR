---
title: tipo de enum deviceComplianceActionType
description: Enumeração de tipo de ação de agendadas
author: tfitzmac
ms.openlocfilehash: 9fd0a8bd045ad04fe0acf55f899e693d7fcce5d0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335683"
---
# <a name="devicecomplianceactiontype-enum-type"></a>tipo de enum deviceComplianceActionType

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Enumeração de tipo de ação de agendadas
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|noAction|0|Nenhuma ação|
|notificação|1|Enviar notificação|
|bloquear|2|Bloquear o dispositivo em AAD|
|retirar|3|Desative o dispositivo|
|apagar|4|Apagar dispositivo|
|removeResourceAccessProfiles|5|Remover o recurso perfis de acesso do dispositivo|
|pushNotification|9|Enviar notificação por push para dispositivos|
|remoteLock|10|Bloquear remotamente o dispositivo|





