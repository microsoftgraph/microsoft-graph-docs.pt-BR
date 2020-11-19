---
title: tipo de enumeração filevaultstate
description: Estado FileVault
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a9aa7c0b11a155597911f64882f5b6d424a2b129
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294519"
---
# <a name="filevaultstate-enum-type"></a>tipo de enumeração filevaultstate

Namespace: microsoft.graph

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




