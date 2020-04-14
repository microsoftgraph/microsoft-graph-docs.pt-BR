---
title: tipo de enumeração vppTokenActionFailureReason
description: Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3b7d236aa9b3cc0b6e20a90b646ba3a95eaf0d3f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463320"
---
# <a name="vpptokenactionfailurereason-enum-type"></a>tipo de enumeração vppTokenActionFailureReason

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|nenhuma|,0|Nenhum.|
|appleFailure|1|Ocorreu um erro no serviço da Apple.|
|internalError|duas|Ocorreu um erro interno.|
|expiredVppToken|3D|Ocorreu um erro porque o token do Apple Volume Purchase Program expirou.|
|expiredApplePushNotificationCertificate|4 |Ocorreu um erro porque o certificado de notificação por push do Apple Volume Purchase Program expirou.|



