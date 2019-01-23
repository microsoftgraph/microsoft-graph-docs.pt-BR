---
title: tipo de enum managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ccd90e4d704a075eaf43650fa765fabf3ab0b99
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410984"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>tipo de enum managedAppClipboardSharingLevel

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|allApps|0|O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não|
|managedAppsWithPasteIn|1|O compartilhamento é permitido entre todos os aplicativos gerenciados com Colar no habilitado|
|managedApps|2|O compartilhamento é permitido entre todos os aplicativos gerenciados|
|bloqueado|3|Compartilhamento entre aplicativos está desabilitado|




