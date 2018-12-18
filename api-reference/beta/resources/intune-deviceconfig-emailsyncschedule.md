---
title: tipo de enum emailSyncSchedule
description: Valores possíveis para a agenda de sincronização de email.
author: tfitzmac
ms.openlocfilehash: f0e6673064f7e483756dfcfec8ce074e809dfcf4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308677"
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





