---
title: tipo de enumeração advancedBitLockerState
description: Estado do BitLocker avançado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5e68f3b608548b5dfd8eb942799a64a4147b6467
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522773"
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
|noUserConsent|1 |O usuário nunca deu o consentimento para a criptografia|
|osVolumeUnprotected|2 |Foi detectado um volume de sistema operacional desprotegido|
|osVolumeTpmRequired|4 |TPM não usado para proteção do volume de so, mas é exigido por política|
|osVolumeTpmOnlyRequired|8 |A proteção somente TPM não é usada para o volume de so, mas é necessária para a política|
|osVolumeTpmPinRequired|16 |TPM + proteção de PIN não usada para o volume de sistema operacional, mas é necessária para a política|
|osVolumeTpmStartupKeyRequired|32|TPM + proteção de chave de inicialização não usada para o volume de sistema operacional, mas é necessária para a política|
|osVolumeTpmPinStartupKeyRequired|64|TPM + PIN + chave de inicialização não usado para o volume de so, mas é exigido pela política|
|osVolumeEncryptionMethodMismatch|128|O método de criptografia do volume de so é diferente daquele definido por política|
|recoveryKeyBackupFailed|256|Falha no backup da chave de recuperação|
|fixedDriveNotEncrypted|512|Unidade fixa não criptografada|
|fixedDriveEncryptionMethodMismatch|1024|O método de criptografia de unidade fixa é diferente daquele definido por política|
|loggedOnUserNonAdmin|2048|O usuário conectado não é administrador. Isso exige que a política "AllowStandardUserEncryption" seja definida como 1|
|windowsRecoveryEnvironmentNotConfigured|4096|WinRE não configurado|
|tpmNotAvailable|8192|O TPM não está disponível para o BitLocker. Isso significa que o TPM não está presente, ou a substituição do registro não disponível do TPM está definida ou o sistema operacional do host está na unidade de capacidade portátil/Roma|
|tpmNotReady|16384|O TPM não está pronto para o BitLocker|
|networkError|32768|Rede não disponível. Isso é necessário para o backup da chave de recuperação. Isso é reportado para dispositivos compatíveis com criptografia de unidade|




