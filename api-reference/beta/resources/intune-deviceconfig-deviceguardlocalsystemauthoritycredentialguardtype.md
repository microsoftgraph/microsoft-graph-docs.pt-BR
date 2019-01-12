---
title: tipo de enum deviceGuardLocalSystemAuthorityCredentialGuardType
description: Valores possíveis de configurações do protetor de credencial.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d284b81632c5ba48fa4c658719203a74fdf52837
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952738"
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





