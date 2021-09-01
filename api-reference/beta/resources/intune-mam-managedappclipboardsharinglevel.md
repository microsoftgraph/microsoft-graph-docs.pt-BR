---
title: Tipo de número managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7b6bc0cb68b28d154d7674246dd305e451623239
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58821098"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>Tipo de número managedAppClipboardSharingLevel

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|allApps|0|O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não|
|managedAppsWithPasteIn|1|O compartilhamento é permitido entre todos os aplicativos gerenciados com a pasta habilitada|
|managedApps|2|O compartilhamento é permitido entre todos os aplicativos gerenciados|
|blocked|3|O compartilhamento entre aplicativos está desabilitado|



