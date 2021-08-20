---
title: Tipo denum fileVaultState
description: Estado FileVault
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9e77c0005dc7dd7cab430fa628cc034919e9fce9cbc3f9171c4bee3846c7c12a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249990"
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
|driveEncryptedByUser|1 |FileVault foi habilitado pelo usuário e não está sendo gerenciado pela política|
|userDeferredEncryption|2|A política FileVault é instalada com êxito, mas o usuário não iniciou a criptografia|
|escrowNotEnabled|4 |A escrow da chave de recuperação FileVault não está habilitada|




