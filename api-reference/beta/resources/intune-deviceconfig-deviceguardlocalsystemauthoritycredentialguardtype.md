---
title: tipo de enumeração deviceGuardLocalSystemAuthorityCredentialGuardType
description: Valores possíveis das configurações do Credential Guard.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 284f0fd4256a3e7f70cc463eecd6ca9655c7ec04
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947012"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a>tipo de enumeração deviceGuardLocalSystemAuthorityCredentialGuardType

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis das configurações do Credential Guard.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|Desativa o Credential Guard remotamente, se configurado anteriormente sem bloqueio de UEFI.|
|enableWithUEFILock|1|Ativa o Credential Guard com bloqueio de UEFI.|
|enableWithoutUEFILock|duas|Ativa o Credential Guard sem bloqueio de UEFI.|




