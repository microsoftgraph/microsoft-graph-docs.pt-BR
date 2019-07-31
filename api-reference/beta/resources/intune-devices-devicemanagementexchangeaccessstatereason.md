---
title: tipo de enumeração deviceManagementExchangeAccessStateReason
description: Motivo do estado de acesso ao Exchange do dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d6761af448b51c9c434472c4ad43978d34b1b1b6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968455"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>tipo de enumeração deviceManagementExchangeAccessStateReason

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Motivo do estado de acesso ao Exchange do dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|,0|Nenhum motivo de estado de acesso descoberto do Exchange|
|desconhecido|1|Razão do estado de acesso desconhecido|
|exchangeGlobalRule|duas|Estado de acesso determinado pela regra global do Exchange|
|exchangeIndividualRule|3D|Estado de acesso determinado pela regra individual do Exchange|
|exchangeDeviceRule|quatro|Estado de acesso determinado pela regra de dispositivo do Exchange|
|exchangeUpgrade|0,5|Estado de acesso devido à atualização do Exchange|
|exchangeMailboxPolicy|6|Estado de acesso determinado pela política de caixa de correio do Exchange|
|outro|178|Estado de acesso determinado pelo Exchange|
|com|8 |Estado de acesso concedido por desafio de conformidade|
|incompatível|9 |Estado de acesso revogado pelo desafio de conformidade|
|Não registrado|10 |Estado de acesso revogado pelo desafio de gerenciamento|
|unknownLocation|3,6|Estado de acesso devido à localização desconhecida|
|mfaRequired|Treze|Estado de acesso devido ao desafio da MFA|
|azureADBlockDueToAccessPolicy|14|Estado de acesso revogado pela política de acesso AAD|
|compromisedPassword|15|Estado de acesso revogado por senha comprometida|
|deviceNotKnownWithManagedApp|dezesseis|Estado de acesso revogado por desafio de aplicativo gerenciado|





