---
title: tipo de enumeração androidDeviceOwnerRequiredPasswordType
description: Política de proprietário do dispositivo Android tipo de senha exigido.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d3df49d6ed508a8d9860c0bb37a234c9fd6e5c2c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968693"
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
|obrigatório|1 |Deve haver uma senha definida, mas não há restrições no tipo.|
|numéricos|2 |Pelo menos numérico.|
|numericComplex|3 |Pelo menos numérico sem sequências de repetição ou ordenadas.|
|caracteres|4 |Pelo menos a senha alfabética.|
|tecla|5 |Pelo menos a senha alfanumérica|
|alphanumericWithSymbols|6 |Pelo menos alfanumérico com símbolos.|
|lowSecurityBiometric|7 |Senha com base em Biometria de segurança baixa necessária.|
|customPassword|8 |Senha personalizada definida pelo administrador.|






