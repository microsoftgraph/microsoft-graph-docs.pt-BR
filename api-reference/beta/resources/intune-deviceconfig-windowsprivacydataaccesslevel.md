---
title: tipo de enumeração windowsPrivacyDataAccessLevel
description: Determine o nível de acesso à categoria de dados de privacidade do Windows específica.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e2cdf124d3da6bf2c08954365a87ae0a97b05267
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159063"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>tipo de enumeração windowsPrivacyDataAccessLevel

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Determine o nível de acesso à categoria de dados de privacidade do Windows específica.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|Nenhum nível de acesso especificado, sem tentativas. O dispositivo pode se comportar como no UserInControl ou no ForceAllow. Pode depender que os dados de privacidade foram acessados, versões do Windows e outros fatores.|
|forceAllow|1|Os aplicativos terão permissão para acessar os dados de privacidade especificados.|
|forceDeny|duas|Os aplicativos serão negados para acessar os dados de privacidade especificados.|
|userInControl|3D|Os usuários serão solicitados quando os aplicativos tentarem acessar dados de privacidade especificados.|




