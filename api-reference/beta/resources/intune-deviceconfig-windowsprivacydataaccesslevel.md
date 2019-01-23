---
title: tipo de enum windowsPrivacyDataAccessLevel
description: Determine o nível de acesso a categoria de dados de privacidade Windows específica.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b5d6fed0897b22a6a6b478dc5d2b7954faca42b2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410620"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>tipo de enum windowsPrivacyDataAccessLevel

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Determine o nível de acesso a categoria de dados de privacidade Windows específica.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|não-configuradas|0|Nenhum nível de acesso não especificado, nenhum propósitos. Dispositivo pode se comportam tanto como UserInControl ou ForceAllow. Ele pode depender os dados de privacidade foram acessados, versões do Windows e outros fatores.|
|forceAllow|1|Aplicativos poderão acessar os dados de privacidade especificado.|
|forceDeny|2|Aplicativos serão negados para acessar os dados de privacidade especificado.|
|userInControl|3|Os usuários serão solicitados quando apps tentam acessar os dados de privacidade especificado.|




