---
title: tipo de enumeração deviceManagementExchangeAccessStateReason
description: Motivo do estado de acesso ao Exchange do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c014afbf22c58f89f8b8926058e28a5ca2d1a1d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252032"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>tipo de enumeração deviceManagementExchangeAccessStateReason

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



