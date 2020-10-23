---
title: tipo de enumeração androidDeviceOwnerRequiredPasswordType
description: Política de proprietário do dispositivo Android tipo de senha exigido.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 09714a743c441058f0a87ff9d26b864a28022b96
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707833"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>tipo de enumeração androidDeviceOwnerRequiredPasswordType

Namespace: microsoft.graph

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





