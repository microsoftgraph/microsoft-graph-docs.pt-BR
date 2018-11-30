---
title: tipo de enum emailSyncSchedule
description: Valores possíveis para a agenda de sincronização de email.
ms.openlocfilehash: 48c5d433815d5f27d018d97ac479641146754669
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033298"
---
# <a name="emailsyncschedule-enum-type"></a>tipo de enum emailSyncSchedule

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis para a agenda de sincronização de email.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|Definido pelo usuário, valor padrão, sem intenção.|
|asMessagesArrive|1|Sincronizar à medida que chegam mensagens.|
|Manual|2|Sincronize manualmente.|
|fifteenMinutes|3|Sincronizar a cada 15 minutos.|
|thirtyMinutes|4|Sincronizar a cada 30 minutos.|
|sixtyMinutes|5|Sincronizar a cada 60 minutos.|
|basedOnMyUsage|6|Sincronizar com base no meu uso.|





