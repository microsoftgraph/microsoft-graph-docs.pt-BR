---
title: Tipo denum vppTokenActionFailureReason
description: Possíveis tipos de motivos para uma falha de ação de token do Programa de Compra de Volume da Apple.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ae12cb78ac9628ffda03ef4b2835f6ef40832e48
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039053"
---
# <a name="vpptokenactionfailurereason-enum-type"></a>Tipo denum vppTokenActionFailureReason

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Possíveis tipos de motivos para uma falha de ação de token do Programa de Compra de Volume da Apple.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|0|Nenhum.|
|appleFailure|1|Houve um erro no serviço da Apple.|
|internalError|2|Houve um erro interno.|
|expiredVppToken|3|Houve um erro porque o token do Programa de Compra de Volume da Apple expirou.|
|expiredApplePushNotificationCertificate|4 |Houve um erro porque o certificado de Notificação por Push do Programa de Compra de Volume da Apple expirou.|



