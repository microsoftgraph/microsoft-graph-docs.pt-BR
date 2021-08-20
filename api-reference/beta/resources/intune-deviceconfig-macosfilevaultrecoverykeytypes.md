---
title: Tipo de número macOSFileVaultRecoveryKeyTypes
description: Tipos de chave de recuperação para macOS FileVault
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c92bec5d4ad5f94e6990c537defe7eb6488b4694bc3f3a5bb4483c716dcaa19d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54198322"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a>Tipo de número macOSFileVaultRecoveryKeyTypes

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipos de chave de recuperação para macOS FileVault

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|Valor padrão do dispositivo, sem intenção.|
|institutionalRecoveryKey|1 |Uma chave de recuperação institucional é como uma chave de recuperação "mestre" que pode ser usada para desbloquear qualquer dispositivo cuja senha foi perdida.|
|personalRecoveryKey|2|Uma chave de recuperação pessoal é um código exclusivo que pode ser usado para desbloquear o dispositivo do usuário, mesmo que a senha do dispositivo seja perdida.|




