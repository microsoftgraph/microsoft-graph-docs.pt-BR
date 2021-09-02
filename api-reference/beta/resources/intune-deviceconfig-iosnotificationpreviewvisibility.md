---
title: Tipo de número iosNotificationPreviewVisibility
description: Determina quando as visualizações de notificação ficam visíveis em um dispositivo iOS. As visualizações podem incluir coisas como texto (de Mensagens e Email) e detalhes do convite (do Calendário). Quando configurado, ele substituirá as configurações de visualização definidas pelo usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3a3f7426134ecf4a5fec3f71cdc33654df292b30
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58759663"
---
# <a name="iosnotificationpreviewvisibility-enum-type"></a>Tipo de número iosNotificationPreviewVisibility

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Determina quando as visualizações de notificação ficam visíveis em um dispositivo iOS. As visualizações podem incluir coisas como texto (de Mensagens e Email) e detalhes do convite (do Calendário). Quando configurado, ele substituirá as configurações de visualização definidas pelo usuário.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|As configurações de visualização de notificação não serão substituídas.|
|alwaysShow|1|Sempre mostrar visualizações de notificação.|
|hideWhenLocked|2|Mostrar visualizações de notificação somente quando o dispositivo estiver desbloqueado.|
|neverShow|3|Nunca mostrar visualizações de notificação.|



