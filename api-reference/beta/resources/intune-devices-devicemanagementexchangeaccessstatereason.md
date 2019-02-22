---
title: tipo de enumeração deviceManagementExchangeAccessStateReason
description: Motivo do estado de acesso ao Exchange do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c788a08e09816683ed575898ee5f36cba241a8bf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175259"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>tipo de enumeração deviceManagementExchangeAccessStateReason

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Motivo do estado de acesso ao Exchange do dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|,0|Nenhum motivo de estado de acesso descoberto do Exchange|
|unknown|1|Razão do estado de acesso desconhecido|
|exchangeGlobalRule|duas|Estado de acesso determinado pela regra global do Exchange|
|exchangeIndividualRule|3D|Estado de acesso determinado pela regra individual do Exchange|
|exchangeDeviceRule|quatro|Estado de acesso determinado pela regra de dispositivo do Exchange|
|exchangeUpgrade|0,5|Estado de acesso devido à atualização do Exchange|
|exchangeMailboxPolicy|6|Estado de acesso determinado pela política de caixa de correio do Exchange|
|outro|178|Estado de acesso determinado pelo Exchange|
|com|8|Estado de acesso concedido por desafio de conformidade|
|inCompatível|241|Estado de acesso revogado pelo desafio de conformidade|
|Não registrado|254|Estado de acesso revogado pelo desafio de gerenciamento|
|unknownLocation|3,6|Estado de acesso devido à localização desconhecida|
|mfaRequired|Treze|Estado de acesso devido ao desafio da MFA|
|azureADBlockDueToAccessPolicy|14|Estado de acesso revogado pela política de acesso AAD|
|compromisedPassword|15|Estado de acesso revogado por senha comprometida|
|deviceNotKnownWithManagedApp|dezesseis|Estado de acesso revogado por desafio de aplicativo gerenciado|




