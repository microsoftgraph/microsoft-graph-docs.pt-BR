---
title: Tipo de número iosNotificationPreviewVisibility
description: Determina quando as visualizações de notificação ficam visíveis em um dispositivo iOS. As visualizações podem incluir coisas como texto (de Mensagens e Email) e detalhes do convite (do Calendário). Quando configurado, ele substituirá as configurações de visualização definidas pelo usuário.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d95630b32e451e762ab7848d96f781346e2f3298
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59131410"
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



