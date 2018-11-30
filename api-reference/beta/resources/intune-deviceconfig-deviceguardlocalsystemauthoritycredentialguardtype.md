---
title: tipo de enum deviceGuardLocalSystemAuthorityCredentialGuardType
description: Valores possíveis de configurações do protetor de credencial.
ms.openlocfilehash: 73668ec4d6d5026402757fae3443da4540fb374c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033188"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a>tipo de enum deviceGuardLocalSystemAuthorityCredentialGuardType

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis de configurações do protetor de credencial.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|não-configuradas|0|Desativa a credencial Guard remotamente se configurado anteriormente sem bloqueio UEFI.|
|enableWithUEFILock|1|Ativa o protetor de credencial com lock UEFI.|
|enableWithoutUEFILock|2|Ativa o protetor de credencial sem bloqueio UEFI.|





