---
title: tipo de enum deviceManagementExchangeAccessStateReason
description: Motivo de estado de acesso do Exchange de dispositivo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 96bcc60daa0ec69788856413bf1d253d8b0cabfc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834784"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>tipo de enum deviceManagementExchangeAccessStateReason

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Motivo de estado de acesso do Exchange de dispositivo.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|nenhum|0|Não há motivo de estado acesso descoberto do Exchange|
|unknown|1|Motivo de estado de acesso desconhecido|
|exchangeGlobalRule|2|Estado de acesso determinado pela regra Global do Exchange|
|exchangeIndividualRule|3|Estado de acesso determinado pela regra Individual do Exchange|
|exchangeDeviceRule|4|Estado de acesso determinado pela regra de dispositivo do Exchange|
|exchangeUpgrade|5|Estado de acesso devido à atualização do Exchange|
|exchangeMailboxPolicy|6|Estado de acesso determinado pela diretiva de caixa de correio do Exchange|
|outros|7|Estado de acesso determinado pelo Exchange|
|compatível com|8|Estado de acesso concedido pelo desafio de conformidade|
|notCompliant|9|Estado de acesso revogado pelo desafio de conformidade|
|notEnrolled|10|Estado de acesso revogado pelo desafio de gerenciamento|
|unknownLocation|12|Estado de acesso devido ao local desconhecido|
|mfaRequired|13|Estado de acesso devido ao desafio MFA|
|azureADBlockDueToAccessPolicy|14|Estado de acesso revogado pela política de acesso AAD|
|compromisedPassword|15|Estado de acesso revogado por senha comprometida|
|deviceNotKnownWithManagedApp|16|Estado de acesso revogado pelo desafio de aplicativo gerenciado|



