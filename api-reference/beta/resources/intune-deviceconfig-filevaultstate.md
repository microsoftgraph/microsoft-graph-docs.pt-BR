---
title: Tipo denum fileVaultState
description: Estado FileVault
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1d9e037eb75fa331e082db5ca19e213c91a927c8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075491"
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



