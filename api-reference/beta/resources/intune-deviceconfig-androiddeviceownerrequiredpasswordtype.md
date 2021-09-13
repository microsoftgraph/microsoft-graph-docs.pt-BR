---
title: tipo de número androidDeviceOwnerRequiredPasswordType
description: A política de Proprietário de Dispositivo Android exigia o tipo de senha.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c3fb30d71826a273ebd1e128d292508f76bfe7a4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023616"
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
|obrigatório|1|Deve haver um conjunto de senhas, mas não há restrições ao tipo.|
|numeric|2|Pelo menos numérico.|
|numericComplex|3|Pelo menos numérico sem sequências repetidas ou ordenadas.|
|alfabético|4 |Pelo menos senha alfabética.|
|alfanumérico|5 |Pelo menos senha alfanumérica|
|alphanumericWithSymbols|6 |Pelo menos alfanumérico com símbolos.|
|lowSecurityBiometric|7 |Senha de baixa biometria baseada em segurança necessária.|
|customPassword|8 |Senha personalizada definida pelo administrador.|



