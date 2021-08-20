---
title: Tipo denum vppTokenActionFailureReason
description: Possíveis tipos de motivos para uma falha de ação de token do Programa de Compra de Volume da Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 920b28aed62eac3b603773e5024d4d8ed5d3f9beff453e4b9f185d6d7f103e8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54133079"
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
|appleFailure|1 |Houve um erro no serviço da Apple.|
|internalError|2|Houve um erro interno.|
|expiredVppToken|3 |Houve um erro porque o token do Programa de Compra de Volume da Apple expirou.|
|expiredApplePushNotificationCertificate|4 |Houve um erro porque o certificado de Notificação por Push do Programa de Compra de Volume da Apple expirou.|




