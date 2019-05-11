---
title: tipo de enumeração androidDeviceOwnerRequiredPasswordType
description: Política de proprietário do dispositivo Android tipo de senha exigido.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc6d81a71fe01addb6111252b28aee01072fe0dd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949063"
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




