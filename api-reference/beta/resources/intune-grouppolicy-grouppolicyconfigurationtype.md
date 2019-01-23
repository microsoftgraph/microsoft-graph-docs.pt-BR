---
title: tipo de enum groupPolicyConfigurationType
description: Tipo de configuração de diretiva de grupo
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 372a5bd5656510c43b388bac128cba4bc46c0988
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429086"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a>tipo de enum groupPolicyConfigurationType

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Tipo de configuração de diretiva de grupo

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Política|0|O tipo de política não tatuam o valor, o que significa que o valor é removido, permitindo que o valor original de configuração a ser usado. O tipo de política substitui a definição de configuração de aplicativo para que o aplicativo sempre seja ciente do valor. O tipo de política impede que o usuário modifique o valor por meio da interface do usuário do aplicativo.|
|preference|1|O tipo de preferência tatuam o valor, o que significa que o valor não é removido do registro. O tipo de preferência substituirá o usuário configurado valor e não retém o valor anterior. O tipo de preferência não impede que o usuário modificar o valor por meio da interface do usuário do aplicativo.|




