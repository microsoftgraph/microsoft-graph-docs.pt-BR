---
title: Tipo denum fileVaultState
description: Estado FileVault
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 942612457d21b587ccfcfff8720216ade2e1be72
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58795547"
---
# <a name="filevaultstate-enum-type"></a>Tipo denum fileVaultState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado FileVault

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|sucesso|0|Sucesso do estado FileVault|
|driveEncryptedByUser|1|FileVault foi habilitado pelo usuário e não está sendo gerenciado pela política|
|userDeferredEncryption|2|A política FileVault é instalada com êxito, mas o usuário não iniciou a criptografia|
|escrowNotEnabled|4 |A escrow da chave de recuperação FileVault não está habilitada|



