---
title: tipo de enumeração androidDeviceOwnerRequiredPasswordType
description: Política de proprietário do dispositivo Android tipo de senha exigido.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e6d783f8bdf5faeed2d3e10a9286a897c8d85783
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42796983"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>tipo de enumeração androidDeviceOwnerRequiredPasswordType

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Política de proprietário do dispositivo Android tipo de senha exigido.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|Valor padrão do dispositivo, sem intenção.|
|obrigatório|1|Deve haver uma senha definida, mas não há restrições no tipo.|
|numéricos|duas|Pelo menos numérico.|
|numericComplex|3D|Pelo menos numérico sem sequências de repetição ou ordenadas.|
|caracteres|4 |Pelo menos a senha alfabética.|
|tecla|5 |Pelo menos a senha alfanumérica|
|alphanumericWithSymbols|6 |Pelo menos alfanumérico com símbolos.|
|lowSecurityBiometric|7 |Senha com base em Biometria de segurança baixa necessária.|
|customPassword|8 |Senha personalizada definida pelo administrador.|



