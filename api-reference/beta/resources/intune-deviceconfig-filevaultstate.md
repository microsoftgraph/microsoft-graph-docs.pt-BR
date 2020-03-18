---
title: tipo de enumeração filevaultstate
description: Estado FileVault
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1efe284a4d6bad3685c6fbf9c4003153a3aca913
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791762"
---
# <a name="filevaultstate-enum-type"></a>tipo de enumeração filevaultstate

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado FileVault

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|sucesso|,0|Êxito no estado FileVault|
|driveEncryptedByUser|1|O FileVault foi habilitado pelo usuário e não está sendo gerenciado por política|
|userDeferredEncryption|duas|A política do FileVault foi instalada com êxito, mas o usuário não iniciou a criptografia|
|escrowNotEnabled|4 |A caução da chave de recuperação FileVault não está habilitada|



