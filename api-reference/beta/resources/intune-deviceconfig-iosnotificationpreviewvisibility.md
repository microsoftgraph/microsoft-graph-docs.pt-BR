---
title: tipo de enumeração iosNotificationPreviewVisibility
description: Determina quando as visualizações de notificação são visíveis em um dispositivo iOS. As visualizações podem incluir itens como texto (de mensagens e email) e detalhes do convite (do calendário). Quando configurado, ele substituirá as configurações de visualização definidas pelo usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 607e771ce83858cd22892efa9a377b7997142a24
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301475"
---
# <a name="iosnotificationpreviewvisibility-enum-type"></a>tipo de enumeração iosNotificationPreviewVisibility

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Determina quando as visualizações de notificação são visíveis em um dispositivo iOS. As visualizações podem incluir itens como texto (de mensagens e email) e detalhes do convite (do calendário). Quando configurado, ele substituirá as configurações de visualização definidas pelo usuário.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|As configurações de visualização de notificação não serão substituídas.|
|alwaysShow|1|Sempre mostrar visualizações de notificação.|
|hideWhenLocked|duas|Mostrar apenas as visualizações de notificação quando o dispositivo estiver desbloqueado.|
|neverShow|3D|Nunca mostrar visualizações de notificação.|




