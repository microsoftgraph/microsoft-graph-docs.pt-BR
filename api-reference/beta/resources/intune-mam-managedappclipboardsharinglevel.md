---
title: tipo de enumeração managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 97e5e74b9d8f039e75df61791ef8dea945e49818
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527962"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>tipo de enumeração managedAppClipboardSharingLevel

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|todos os aplicativos|,0|O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não|
|managedAppsWithPasteIn|1 |O compartilhamento é permitido entre todos os aplicativos gerenciados com colar ativado|
|managedApps|2 |O compartilhamento é permitido entre todos os aplicativos gerenciados|
|bloqueou|3 |O compartilhamento entre aplicativos está desabilitado|



