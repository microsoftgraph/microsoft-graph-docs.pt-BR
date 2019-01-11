---
title: tipo de enum windowsPrivacyDataAccessLevel
description: Determine o nível de acesso a categoria de dados de privacidade Windows específica.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 74ab32a703422203fec7a6c9ed1bc035e01949a9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888771"
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





