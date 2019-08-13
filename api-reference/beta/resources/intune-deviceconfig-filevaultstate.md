---
title: tipo de enumeração filevaultstate
description: Estado FileVault
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 54e8076dc4b4f6ab20f7790d2a650de6c07aa702
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325565"
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



