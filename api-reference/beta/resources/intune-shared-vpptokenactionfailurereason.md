---
title: tipo de enumeração vppTokenActionFailureReason
description: Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8765d0dd62579f470133e81005ff995638e00a5d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42767096"
---
# <a name="vpptokenactionfailurereason-enum-type"></a>tipo de enumeração vppTokenActionFailureReason

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|,0|Nenhum.|
|appleFailure|1|Ocorreu um erro no serviço da Apple.|
|internalError|duas|Ocorreu um erro interno.|
|expiredVppToken|3D|Ocorreu um erro porque o token do Apple Volume Purchase Program expirou.|
|expiredApplePushNotificationCertificate|4 |Ocorreu um erro porque o certificado de notificação por push do Apple Volume Purchase Program expirou.|



