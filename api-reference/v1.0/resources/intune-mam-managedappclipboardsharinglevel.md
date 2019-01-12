---
title: tipo de enum managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 349f0ee08b8e3bff4e627c58318e2c21fa00847c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946781"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>tipo de enum managedAppClipboardSharingLevel

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|allApps|0|O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não|
|managedAppsWithPasteIn|1|O compartilhamento é permitido entre todos os aplicativos gerenciados com Colar no habilitado|
|managedApps|2|O compartilhamento é permitido entre todos os aplicativos gerenciados|
|bloqueado|3|Compartilhamento entre aplicativos está desabilitado|



