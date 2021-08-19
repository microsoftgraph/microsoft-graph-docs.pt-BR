---
title: tipo de número androidDeviceOwnerRequiredPasswordType
description: A política de Proprietário de Dispositivo Android exigia o tipo de senha.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d5fdb65510bcd287494b3966ca00bbe7f25b0a2fd5720338030bc1bcf8c11a64
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54183216"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>tipo de número androidDeviceOwnerRequiredPasswordType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A política de Proprietário de Dispositivo Android exigia o tipo de senha.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Valor padrão do dispositivo, sem intenção.|
|obrigatório|1 |Deve haver um conjunto de senhas, mas não há restrições ao tipo.|
|numeric|2|Pelo menos numérico.|
|numericComplex|3 |Pelo menos numérico sem sequências repetidas ou ordenadas.|
|alfabético|4 |Pelo menos senha alfabética.|
|alfanumérico|5 |Pelo menos senha alfanumérica|
|alphanumericWithSymbols|6 |Pelo menos alfanumérico com símbolos.|
|lowSecurityBiometric|7 |Senha de baixa biometria baseada em segurança necessária.|
|customPassword|8 |Senha personalizada definida pelo administrador.|




