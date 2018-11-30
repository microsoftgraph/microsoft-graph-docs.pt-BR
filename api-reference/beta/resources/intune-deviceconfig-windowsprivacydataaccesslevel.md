---
title: tipo de enum windowsPrivacyDataAccessLevel
description: Determine o nível de acesso a categoria de dados de privacidade Windows específica.
ms.openlocfilehash: 09db03706795cc2aba4cc0c93dce87dc7069cd3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040905"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>tipo de enum windowsPrivacyDataAccessLevel

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Determine o nível de acesso a categoria de dados de privacidade Windows específica.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|não-configuradas|0|Nenhum nível de acesso não especificado, nenhum propósitos. Dispositivo pode se comportam tanto como UserInControl ou ForceAllow. Ele pode depender os dados de privacidade foram acessados, versões do Windows e outros fatores.|
|forceAllow|1|Aplicativos poderão acessar os dados de privacidade especificado.|
|forceDeny|2|Aplicativos serão negados para acessar os dados de privacidade especificado.|
|userInControl|3|Os usuários serão solicitados quando apps tentam acessar os dados de privacidade especificado.|





