---
title: tipo de enumeração groupPolicyConfigurationType
description: Tipo de configuração da política de grupo
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4428493cc0a76fd22ee7155cacda22d38eb10204
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975893"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a>tipo de enumeração groupPolicyConfigurationType

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de configuração da política de grupo

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|política|,0|O tipo de política não é de Tattoo o valor, o que significa que o valor é removido, permitindo que o valor de configuração original seja usado. O tipo de política substitui a definição de configuração de aplicativo para que o aplicativo sempre saiba o valor. O tipo de política impede que o usuário modifique o valor por meio da interface do usuário do aplicativo.|
|preferência|1|O tipo de preferência tem o valor de Tattoo, o que significa que o valor não é removido do registro. O tipo de preferência substituirá o valor configurado pelo usuário e não manterá o valor anterior. O tipo de preferência não impede que o usuário modifique o valor por meio da interface do usuário do aplicativo.|





