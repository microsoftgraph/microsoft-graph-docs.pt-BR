---
title: tipo de enumeração androidDeviceOwnerRequiredPasswordType
description: Política de proprietário do dispositivo Android tipo de senha exigido.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 376e33edac921f6771d76a45622a58bca3076c5c
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572331"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>tipo de enumeração androidDeviceOwnerRequiredPasswordType

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Política de proprietário do dispositivo Android tipo de senha exigido.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|Valor padrão do dispositivo, sem intenção.|
|obrigatório|1|Deve haver uma senha definida, mas não há restrições no tipo.|
|numéricos|duas|Pelo menos numérico.|
|numericComplex|3D|Pelo menos numérico sem sequências de repetição ou ordenadas.|
|caracteres|quatro|Pelo menos a senha alfabética.|
|tecla|0,5|Pelo menos a senha alfanumérica|
|alphanumericWithSymbols|6|Pelo menos alfanumérico com símbolos.|
|lowSecurityBiometric|178|Senha com base em Biometria de segurança baixa necessária.|




