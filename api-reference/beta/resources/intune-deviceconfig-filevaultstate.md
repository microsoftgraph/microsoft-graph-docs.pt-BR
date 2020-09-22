---
title: tipo de enumeração filevaultstate
description: Estado FileVault
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4d2e038d5f75f25bb534bfc5923b946d0a0dfd16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994138"
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
|driveEncryptedByUser|1 |O FileVault foi habilitado pelo usuário e não está sendo gerenciado por política|
|userDeferredEncryption|2 |A política do FileVault foi instalada com êxito, mas o usuário não iniciou a criptografia|
|escrowNotEnabled|4 |A caução da chave de recuperação FileVault não está habilitada|






