---
title: tipo de número browserSyncSetting
description: Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings. Opção para impedir a sincronização entre dispositivos, mas permitir a substituição do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ef97db0168971b687d3dac5fb405f5c9482b2a3d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58802779"
---
# <a name="browsersyncsetting-enum-type"></a>tipo de número browserSyncSetting

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings. Opção para impedir a sincronização entre dispositivos, mas permitir a substituição do usuário.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|Padrão – Permitir a sincronização das configurações do navegador entre dispositivos.|
|blockedWithUserOverride|1|Impedir a sincronização das configurações do navegador entre dispositivos do usuário, permitir a substituição do usuário da configuração.|
|blocked|2|Impedir absolutamente a sincronização das configurações do navegador em dispositivos de usuário.|



