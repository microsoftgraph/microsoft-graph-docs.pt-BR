---
title: tipo de enumeração windowsPrivacyDataAccessLevel
description: Determine o nível de acesso à categoria de dados de privacidade do Windows específica.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 96ef43bae6996c3268a3e0d268f80267e192deee
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786247"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>tipo de enumeração windowsPrivacyDataAccessLevel

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Determine o nível de acesso à categoria de dados de privacidade do Windows específica.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|Nenhum nível de acesso especificado, sem tentativas. O dispositivo pode se comportar como no UserInControl ou no ForceAllow. Pode depender que os dados de privacidade foram acessados, versões do Windows e outros fatores.|
|forceAllow|1|Os aplicativos terão permissão para acessar os dados de privacidade especificados.|
|forceDeny|duas|Os aplicativos serão negados para acessar os dados de privacidade especificados.|
|userInControl|3D|Os usuários serão solicitados quando os aplicativos tentarem acessar dados de privacidade especificados.|



