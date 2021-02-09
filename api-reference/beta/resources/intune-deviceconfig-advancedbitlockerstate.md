---
title: Tipo de enum advancedBitLockerState
description: Estado avançado do BitLocker
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8ad93a61e03e923ef1c74121574ee5f4e9a94d36
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153596"
---
# <a name="advancedbitlockerstate-enum-type"></a>Tipo de enum advancedBitLockerState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado avançado do BitLocker

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|sucesso|0|Sucesso avançado do estado do BitLocker|
|noUserConsent|1 |O usuário nunca deu consentimento para Criptografia|
|osVolumeUnprotected|2 |Volume do sistema operacional não protegido detectado|
|osVolumeTpmRequired|4 |O TPM não é usado para proteção do volume do sistema operacional, mas é exigido pela política|
|osVolumeTpmOnlyRequired|8 |A proteção do TPM não é usada para volume do sistema operacional, mas é exigida pela política|
|osVolumeTpmPinRequired|16 |Proteção TPM+PIN não usada para volume do sistema operacional, mas é exigida pela política|
|osVolumeTpmStartupKeyRequired|32|A proteção TPM+Chave de Inicialização não é usada para volume do sistema operacional, mas é exigida pela política|
|osVolumeTpmPinStartupKeyRequired|64|TPM+PIN+Chave de Inicialização não é usado para volume do sistema operacional, mas é exigido pela política|
|osVolumeEncryptionMethodMismatch|128|O método de criptografia do volume do sistema operacional é diferente do definido pela política|
|recoveryKeyBackupFailed|256|Falha no backup da chave de recuperação|
|fixedDriveNotEncrypted|512|Unidade Fixa não criptografada|
|fixedDriveEncryptionMethodMismatch|1024|O método de criptografia da Unidade Fixa é diferente do definido pela política|
|loggedOnUserNonAdmin|2048|O usuário conectado não é administrador. Isso requer a política "AllowStandardUserEncryption" definida como 1|
|windowsRecoveryEnvironmentNotConfigured|4096|O WinRE não está configurado|
|tpmNotAvailable|8192|O TPM não está disponível para o BitLocker. Isso significa que o TPM não está presente ou a substituição do Registro indisponível do TPM está definida ou o sistema operacional host está em uma unidade portátil/acessível|
|tpmNotReady|16384|O TPM não está pronto para o BitLocker|
|networkError|32768|Rede não disponível. Isso é necessário para o backup da chave de recuperação. Isso é relatado para dispositivos compatíveis com a Criptografia de Unidade|




