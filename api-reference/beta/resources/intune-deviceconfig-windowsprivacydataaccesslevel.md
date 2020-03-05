---
title: tipo de enumeração windowsPrivacyDataAccessLevel
description: Determine o nível de acesso à categoria de dados de privacidade do Windows específica.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8ccf26f70cd76a58f2489ae1457b2c15e7c5a2d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525408"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>tipo de enumeração windowsPrivacyDataAccessLevel

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Determine o nível de acesso à categoria de dados de privacidade do Windows específica.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|Nenhum nível de acesso especificado, sem tentativas. O dispositivo pode se comportar como no UserInControl ou no ForceAllow. Pode depender que os dados de privacidade foram acessados, versões do Windows e outros fatores.|
|forceAllow|1 |Os aplicativos terão permissão para acessar os dados de privacidade especificados.|
|forceDeny|2 |Os aplicativos serão negados para acessar os dados de privacidade especificados.|
|userInControl|3 |Os usuários serão solicitados quando os aplicativos tentarem acessar dados de privacidade especificados.|



