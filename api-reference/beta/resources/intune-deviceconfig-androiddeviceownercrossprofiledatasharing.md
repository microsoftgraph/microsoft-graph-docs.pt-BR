---
title: tipo de número androidDeviceOwnerCrossProfileDataSharing
description: Uma enum que representa os valores possíveis para o compartilhamento de dados entre perfis.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2e30b55d7e99e3d33914b666a2088ad29178890a
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348361"
---
# <a name="androiddeviceownercrossprofiledatasharing-enum-type"></a>tipo de número androidDeviceOwnerCrossProfileDataSharing

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma enum que representa os valores possíveis para o compartilhamento de dados entre perfis.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|Não configurado; esse valor é padrão para CROSS_PROFILE_DATA_SHARING_UNSPECIFIED.|
|crossProfileDataSharingBlocked|1|Os dados não podem ser compartilhados do perfil pessoal para o perfil de trabalho e do perfil de trabalho para o perfil pessoal.|
|dataSharingFromWorkToPersonalBlocked|2|Impede que os usuários compartilhem dados do perfil de trabalho para aplicativos no perfil pessoal. Os dados pessoais podem ser compartilhados com aplicativos de trabalho.|
|crossProfileDataSharingAllowed|3|Os dados de qualquer perfil podem ser compartilhados com o outro perfil.|
|unkownFutureValue|4|Valor futuro desconhecido (reservado, não usado agora)|




