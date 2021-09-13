---
title: Tipo de número advancedBitLockerState
description: Estado avançado do BitLocker
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ad5532d92b16fe99be8f0e114e967305324bfcb4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020431"
---
# <a name="advancedbitlockerstate-enum-type"></a>Tipo de número advancedBitLockerState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado avançado do BitLocker

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|sucesso|0|Sucesso avançado do estado do BitLocker|
|noUserConsent|1|O usuário nunca deu consentimento para Criptografia|
|osVolumeUnprotected|2|Volume do sistema operacional não protegido foi detectado|
|osVolumeTpmRequired|4 |O TPM não é usado para proteção do volume do sistema operacional, mas é exigido pela política|
|osVolumeTpmOnlyRequired|8 |Proteção somente TPM não usada para volume do sistema operacional, mas é necessária pela política|
|osVolumeTpmPinRequired|16 |Proteção TPM+PIN não usada para volume do sistema operacional, mas é necessária pela política|
|osVolumeTpmStartupKeyRequired|32|Proteção de chave de inicialização do TPM+não usada para volume do sistema operacional, mas é necessária pela política|
|osVolumeTpmPinStartupKeyRequired|64|TPM+PIN+Chave de Inicialização não usada para volume do sistema operacional, mas é necessária pela política|
|osVolumeEncryptionMethodMismatch|128|O método de criptografia do volume do sistema operacional é diferente do definido pela política|
|recoveryKeyBackupFailed|256|Falha no backup da chave de recuperação|
|fixedDriveNotEncrypted|512|Unidade Fixa não criptografada|
|fixedDriveEncryptionMethodMismatch|1024|O método de criptografia de Unidade Fixa é diferente do definido pela política|
|loggedOnUserNonAdmin|2048|O usuário conectado não é administrador. Isso requer a política "AllowStandardUserEncryption" definida como 1|
|windowsRecoveryEnvironmentNotConfigured|4096|WinRE não está configurado|
|tpmNotAvailable|8192|O TPM não está disponível para o BitLocker. Isso significa que o TPM não está presente, ou a substituição indisponível do Registro do TPM está definida ou o sistema operacional host está em unidade portátil/acessível a roma|
|tpmNotReady|16384|O TPM não está pronto para o BitLocker|
|networkError|32768|Rede não disponível. Isso é necessário para backup de teclas de recuperação. Isso é relatado para dispositivos compatíveis com Criptografia de Unidade|



