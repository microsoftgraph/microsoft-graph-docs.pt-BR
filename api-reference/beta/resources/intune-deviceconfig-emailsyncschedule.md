---
title: tipo de enum emailSyncSchedule
description: Valores possíveis para a agenda de sincronização de email.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8285b9a34e208b86b7c53c38e6aa015fd8c37560
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425180"
---
# <a name="emailsyncschedule-enum-type"></a>tipo de enum emailSyncSchedule

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

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




