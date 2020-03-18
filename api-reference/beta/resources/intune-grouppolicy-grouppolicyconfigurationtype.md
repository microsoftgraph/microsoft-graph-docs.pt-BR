---
title: tipo de enumeração groupPolicyConfigurationType
description: Tipo de configuração da política de grupo
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 38e0eaef1fb4f76584fc791d0b5847832f186dbf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783099"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a>tipo de enumeração groupPolicyConfigurationType

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de configuração da política de grupo

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|política|,0|O tipo de política não é de Tattoo o valor, o que significa que o valor é removido, permitindo que o valor de configuração original seja usado. O tipo de política substitui a definição de configuração de aplicativo para que o aplicativo sempre saiba o valor. O tipo de política impede que o usuário modifique o valor por meio da interface do usuário do aplicativo.|
|preferência|1|O tipo de preferência tem o valor de Tattoo, o que significa que o valor não é removido do registro. O tipo de preferência substituirá o valor configurado pelo usuário e não manterá o valor anterior. O tipo de preferência não impede que o usuário modifique o valor por meio da interface do usuário do aplicativo.|



