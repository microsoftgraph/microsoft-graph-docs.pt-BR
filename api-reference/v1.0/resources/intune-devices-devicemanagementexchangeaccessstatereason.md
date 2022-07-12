---
title: Tipo de enumeração deviceManagementExchangeAccessStateReason
description: Motivo do estado de acesso do Exchange do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f6cc10fd962a43ed87179299f22e48d84c7c13ba
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66736066"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>Tipo de enumeração deviceManagementExchangeAccessStateReason

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Motivo do estado de acesso do Exchange do dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|0|Nenhum motivo de estado de acesso descoberto do Exchange|
|desconhecido|1|Motivo do estado de acesso desconhecido|
|exchangeGlobalRule|2|Estado de acesso determinado pela regra global do Exchange|
|exchangeIndividualRule|3|Estado de acesso determinado pela regra individual do Exchange|
|exchangeDeviceRule|4|Estado de acesso determinado pela regra de dispositivo do Exchange|
|exchangeUpgrade|5|Estado de acesso devido à atualização do Exchange|
|exchangeMailboxPolicy|6 |Estado de acesso determinado pela Política de Caixa de Correio do Exchange|
|Outros|7 |Estado de acesso determinado pelo Exchange|
|Compatível|8 |Estado de acesso concedido pelo desafio de conformidade|
|notCompliant|9 |Estado de acesso revogado pelo desafio de conformidade|
|notEnrolled|10|Estado de acesso revogado pelo desafio de gerenciamento|
|unknownLocation|12 |Estado de acesso devido a um local desconhecido|
|mfaRequired|13|Estado de acesso devido ao desafio de MFA|
|azureADBlockDueToAccessPolicy|14|Estado de Acesso revogado pela Política de Acesso do AAD|
|compromisedPassword|15|Estado de Acesso revogado por senha comprometida|
|deviceNotKnownWithManagedApp|16|Estado de acesso revogado pelo desafio de aplicativo gerenciado|





