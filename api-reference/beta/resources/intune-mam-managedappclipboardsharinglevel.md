---
title: tipo de enum managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 41983b9bb30880768fff0ee02883c32fcb5305a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968411"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>tipo de enum managedAppClipboardSharingLevel

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|allApps|0|O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não|
|managedAppsWithPasteIn|1|O compartilhamento é permitido entre todos os aplicativos gerenciados com Colar no habilitado|
|managedApps|2|O compartilhamento é permitido entre todos os aplicativos gerenciados|
|bloqueado|3|Compartilhamento entre aplicativos está desabilitado|





