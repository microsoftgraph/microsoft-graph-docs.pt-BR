---
title: tipo de enumeração androidDeviceOwnerRequiredPasswordType
description: Política de proprietário do dispositivo Android tipo de senha exigido.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7a94dabb436ec11dd340c15afcbd7ed2f04ddbca
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538634"
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
|caracteres|4 |Pelo menos a senha alfabética.|
|tecla|5 |Pelo menos a senha alfanumérica|
|alphanumericWithSymbols|6 |Pelo menos alfanumérico com símbolos.|
|lowSecurityBiometric|7 |Senha com base em Biometria de segurança baixa necessária.|
|customPassword|8 |Senha personalizada definida pelo administrador.|



