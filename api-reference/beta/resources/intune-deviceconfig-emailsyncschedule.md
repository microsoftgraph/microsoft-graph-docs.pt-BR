---
title: tipo de enum emailSyncSchedule
description: Valores possíveis para a agenda de sincronização de email.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 178cba9e226b7f20e3fd917145e7bbd06f6c3a1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838392"
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





