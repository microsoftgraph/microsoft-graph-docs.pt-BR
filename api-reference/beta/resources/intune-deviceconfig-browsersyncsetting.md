---
title: tipo de enum browserSyncSetting
description: Allow(Not Configured) ou prevent(Block) a sincronização das configurações do navegador de borda da Microsoft. Opção para impedir que está sincronizando entre dispositivos, mas permitir substituição do usuário.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8dce2b82b1eea5e4b06ed0f6949ba6a403b073a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431230"
---
# <a name="browsersyncsetting-enum-type"></a>tipo de enum browserSyncSetting

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Allow(Not Configured) ou prevent(Block) a sincronização das configurações do navegador de borda da Microsoft. Opção para impedir que está sincronizando entre dispositivos, mas permitir substituição do usuário.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|não-configuradas|0|Padrão – permitir entre dispositivos está sincronizando das configurações do navegador.|
|blockedWithUserOverride|1|Impedir a sincronização das configurações do navegador entre dispositivos do usuário, Permitir substituição do usuário de configuração.|
|bloqueado|2|Absolutamente impedir que está sincronizando das configurações do navegador entre dispositivos do usuário.|




