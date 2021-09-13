---
title: Tipo de número managedAppClipboardSharingLevel
description: Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e8c3ba5b99b6f416e77ec41d51439fb3b6550370
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075141"
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



