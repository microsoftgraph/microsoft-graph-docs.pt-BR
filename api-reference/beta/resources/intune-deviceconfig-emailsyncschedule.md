---
title: tipo de número emailSyncSchedule
description: Valores possíveis para agendamento de sincronização de email.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0415b01c743c9edb3cb9f777d86c77446528d7a6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020410"
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



