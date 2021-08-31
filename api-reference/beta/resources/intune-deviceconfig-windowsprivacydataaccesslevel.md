---
title: Tipo de número do windowsPrivacyDataAccessLevel
description: Determine o nível de acesso para a categoria Windows dados de privacidade específicos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5fa4ee09c3e931766fe3f76131841e0d69bdc65d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58793842"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>Tipo de número do windowsPrivacyDataAccessLevel

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Determine o nível de acesso para a categoria Windows dados de privacidade específicos.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|Nenhum nível de acesso especificado, nenhuma intenção. O dispositivo pode se comportar como em UserInControl ou ForceAllow. Pode depender dos dados de privacidade que foram acessados, Windows versões e outros fatores.|
|forceAllow|1|Os aplicativos terão permissão para acessar os dados de privacidade especificados.|
|forceDeny|2|Os aplicativos serão negados para acessar dados de privacidade especificados.|
|userInControl|3|Os usuários serão solicitados quando os aplicativos tentarem acessar dados de privacidade especificados.|



