---
title: tipo de enumeração macOSFileVaultRecoveryKeyTypes
description: Tipos de chave de recuperação para macOS FileVault
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: df4374cdcb56a4400c483fea84d2cf02b3c6c0dc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024168"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a>tipo de enumeração macOSFileVaultRecoveryKeyTypes

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipos de chave de recuperação para macOS FileVault

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|Valor padrão do dispositivo, sem intenção.|
|institutionalRecoveryKey|1 |Uma chave de recuperação institucional é como uma chave de recuperação "mestra" que pode ser usada para desbloquear qualquer dispositivo cuja senha tenha sido perdida.|
|personalRecoveryKey|2 |Uma chave de recuperação pessoal é um código exclusivo que pode ser usado para desbloquear o dispositivo do usuário, mesmo se a senha do dispositivo for perdida.|






