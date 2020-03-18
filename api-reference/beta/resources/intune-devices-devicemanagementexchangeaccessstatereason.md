---
title: tipo de enumeração deviceManagementExchangeAccessStateReason
description: Motivo do estado de acesso ao Exchange do dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 00f9c44237052b4f15917763c6452c1a909543fc
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784920"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>tipo de enumeração deviceManagementExchangeAccessStateReason

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Motivo do estado de acesso ao Exchange do dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|,0|Nenhum motivo de estado de acesso descoberto do Exchange|
|desconhecido|1|Razão do estado de acesso desconhecido|
|exchangeGlobalRule|duas|Estado de acesso determinado pela regra global do Exchange|
|exchangeIndividualRule|3D|Estado de acesso determinado pela regra individual do Exchange|
|exchangeDeviceRule|4 |Estado de acesso determinado pela regra de dispositivo do Exchange|
|exchangeUpgrade|5 |Estado de acesso devido à atualização do Exchange|
|exchangeMailboxPolicy|6 |Estado de acesso determinado pela política de caixa de correio do Exchange|
|outro|7 |Estado de acesso determinado pelo Exchange|
|com|8 |Estado de acesso concedido por desafio de conformidade|
|incompatível|9 |Estado de acesso revogado pelo desafio de conformidade|
|Não registrado|10 |Estado de acesso revogado pelo desafio de gerenciamento|
|unknownLocation|12 |Estado de acesso devido à localização desconhecida|
|mfaRequired|13 |Estado de acesso devido ao desafio da MFA|
|azureADBlockDueToAccessPolicy|14 |Estado de acesso revogado pela política de acesso AAD|
|compromisedPassword|15 |Estado de acesso revogado por senha comprometida|
|deviceNotKnownWithManagedApp|16 |Estado de acesso revogado por desafio de aplicativo gerenciado|



