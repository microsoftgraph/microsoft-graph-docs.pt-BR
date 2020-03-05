---
title: tipo de enumeração vppTokenActionFailureReason
description: Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8b7df30d2673696200b29e14d7c450c41d5a5f8b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523503"
---
# <a name="vpptokenactionfailurereason-enum-type"></a>tipo de enumeração vppTokenActionFailureReason

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Possíveis tipos de motivos para uma falha na ação de token do Apple Volume Purchase Program.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|nenhuma|,0|Nenhum.|
|appleFailure|1 |Ocorreu um erro no serviço da Apple.|
|internalError|2 |Ocorreu um erro interno.|
|expiredVppToken|3 |Ocorreu um erro porque o token do Apple Volume Purchase Program expirou.|
|expiredApplePushNotificationCertificate|4 |Ocorreu um erro porque o certificado de notificação por push do Apple Volume Purchase Program expirou.|



