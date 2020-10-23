---
title: tipo de enumeração advancedBitLockerState
description: Estado do BitLocker avançado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9d4b29f3e60efef15232eccc66bdd2df752a7919
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731952"
---
# <a name="advancedbitlockerstate-enum-type"></a>tipo de enumeração advancedBitLockerState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado do BitLocker avançado

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|sucesso|,0|Êxito no estado do BitLocker avançado|
|noUserConsent|1|O usuário nunca deu o consentimento para a criptografia|
|osVolumeEncryptionMethodMismatch|duas|O método de criptografia do volume de so é diferente daquele definido por política|
|osVolumeTpmRequired|4 |TPM não usado para proteção do volume de so, mas é exigido por política|
|osVolumeTpmOnlyRequired|8 |A proteção somente TPM não é usada para o volume de so, mas é necessária para a política|
|osVolumeTpmPinRequired|16 |TPM + proteção de PIN não usada para o volume de sistema operacional, mas é necessária para a política|
|osVolumeTpmStartupKeyRequired|32|TPM + proteção de chave de inicialização não usada para o volume de sistema operacional, mas é necessária para a política|
|osVolumeTpmPinStartupKeyRequired|64|TPM + PIN + chave de inicialização não usado para o volume de so, mas é exigido pela política|
|osVolumeUnprotected|128|O volume de so desprotegido foi detectado|
|recoveryKeyBackupFailed|256|Falha no backup da chave de recuperação|
|fixedDriveNotEncrypted|512|Unidade fixa não criptografada|
|fixedDriveEncryptionMethodMismatch|1024|O método de criptografia de unidade fixa é diferente daquele definido por política|
|loggedOnUserNonAdmin|2048|O usuário conectado não é administrador. Isso exige que a política "AllowStandardUserEncryption" seja definida como 1|
|windowsRecoveryEnvironmentNotConfigured|4096|WinRE não configurado|
|tpmNotAvailable|8192|O TPM não está disponível para o BitLocker. Isso significa que o TPM não está presente, ou a substituição do registro não disponível do TPM está definida ou o sistema operacional do host está na unidade de capacidade portátil/Roma|
|tpmNotReady|16384|O TPM não está pronto para o BitLocker|
|networkError|32768|Rede não disponível. Isso é necessário para o backup da chave de recuperação. Isso é reportado para dispositivos compatíveis com criptografia de unidade|





