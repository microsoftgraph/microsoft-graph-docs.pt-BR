---
title: tipo de número emailSyncSchedule
description: Valores possíveis para agendamento de sincronização de email.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 899b62b78f99f362732f9b7072d3e4a48eb1fdc6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58802513"
---
# <a name="emailsyncschedule-enum-type"></a>tipo de número emailSyncSchedule

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para agendamento de sincronização de email.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|User Defined, default value, no intent.|
|asMessagesArrive|1|Sincronizar à medida que as mensagens chegam.|
|Manual|2|Sincronizar manualmente.|
|fifteenMinutes|3|Sincronizar a cada quinze minutos.|
|thirtyMinutes|4 |Sincronizar a cada trinta minutos.|
|sixtyMinutes|5 |Sincronizar a cada 60 minutos.|
|basedOnMyUsage|6 |Sincronização com base no meu uso.|



