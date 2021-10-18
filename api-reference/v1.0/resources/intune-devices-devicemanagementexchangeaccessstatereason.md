---
title: Tipo de número deviceManagementExchangeAccessStateReason
description: Motivo Exchange estado do Access do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 87cdf39172f63bf93c0d48850485b1443b9c99bb
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60453832"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>Tipo de número deviceManagementExchangeAccessStateReason

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Motivo Exchange estado do Access do dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|0|Nenhum motivo de estado de acesso descoberto Exchange|
|desconhecido|1|Motivo do estado de acesso desconhecido|
|exchangeGlobalRule|2|Estado de acesso determinado pela Exchange Global|
|exchangeIndividualRule|3|Estado de acesso determinado por Exchange regra individual|
|exchangeDeviceRule|4 |Estado de acesso determinado pela regra Exchange Device|
|exchangeUpgrade|5|Estado de acesso devido Exchange atualização|
|exchangeMailboxPolicy|6 |Estado de acesso determinado pela Exchange de Caixa de Correio|
|other|7 |Estado de acesso determinado por Exchange|
|compatível|8 |Estado de acesso concedido pelo desafio de conformidade|
|notCompliant|9 |Estado de acesso revogado pelo desafio de conformidade|
|notEnrolled|10 |Estado de acesso revogado pelo desafio de gerenciamento|
|unknownLocation|12 |Estado de acesso devido a localização desconhecida|
|mfaRequired|13|Estado de acesso devido ao desafio MFA|
|azureADBlockDueToAccessPolicy|14 |Estado do Access revogado pela política AAD Access|
|compromisedPassword|15 |Estado do Access revogado por senha comprometida|
|deviceNotKnownWithManagedApp|16|Estado de acesso revogado pelo desafio de aplicativo gerenciado|



