---
title: tipo de enumeração filevaultstate
description: Estado FileVault
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8f2fa72d2db91ba000209332aec3d59579cba822
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529995"
---
# <a name="filevaultstate-enum-type"></a>tipo de enumeração filevaultstate

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado FileVault

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|sucesso|,0|Êxito no estado FileVault|
|driveEncryptedByUser|1 |O FileVault foi habilitado pelo usuário e não está sendo gerenciado por política|
|userDeferredEncryption|2 |A política do FileVault foi instalada com êxito, mas o usuário não iniciou a criptografia|
|escrowNotEnabled|4 |A caução da chave de recuperação FileVault não está habilitada|



