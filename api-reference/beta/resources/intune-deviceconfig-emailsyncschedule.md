---
title: tipo de enumeração emailSyncSchedule
description: Valores possíveis para agenda de sincronização de email.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 565cde82689fb8e208f0b7c6463e9a7b647a4d75
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460084"
---
# <a name="emailsyncschedule-enum-type"></a>tipo de enumeração emailSyncSchedule

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para agenda de sincronização de email.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|UserDefined|,0|Definido pelo usuário, valor padrão, sem intenção.|
|asMessagesArrive|1|Sincronizar à medida que as mensagens chegam.|
|Manual|duas|Sincronizar manualmente.|
|fifteenMinutes|3D|Sincronizar a cada quinze minutos.|
|thirtyMinutes|4 |Sincronizar a cada trinta minutos.|
|sixtyMinutes|5 |Sincronizar a cada 60 minutos.|
|basedOnMyUsage|6 |Sincronizar com base no meu uso.|



