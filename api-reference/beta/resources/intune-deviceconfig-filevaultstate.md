---
title: tipo de enumeração filevaultstate
description: Estado FileVault
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f122d62f85f90825f5fe3129ec2a314d5886e6f2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725865"
---
# <a name="filevaultstate-enum-type"></a>tipo de enumeração filevaultstate

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado FileVault

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|sucesso|,0|Êxito no estado FileVault|
|driveEncryptedByUser|1|O FileVault foi habilitado pelo usuário e não está sendo gerenciado por política|
|userDeferredEncryption|duas|A política do FileVault foi instalada com êxito, mas o usuário não iniciou a criptografia|
|escrowNotEnabled|quatro|A caução da chave de recuperação FileVault não está habilitada|







