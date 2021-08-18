---
title: Tipo de número deviceManagementExchangeAccessStateReason
description: Motivo Exchange estado do Access do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2ad09fe55138e194a08565413af909110092ccdd82b9e3cdafe7612b2e33c324
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54150350"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>Tipo de número deviceManagementExchangeAccessStateReason

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Motivo Exchange estado do Access do dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|0|Nenhum motivo de estado de acesso descoberto Exchange|
|desconhecido|1 |Motivo do estado de acesso desconhecido|
|exchangeGlobalRule|2|Estado de acesso determinado pela Exchange Global|
|exchangeIndividualRule|3 |Estado de acesso determinado por Exchange regra individual|
|exchangeDeviceRule|4 |Estado de acesso determinado pela regra Exchange Device|
|exchangeUpgrade|5 |Estado de acesso devido Exchange atualização|
|exchangeMailboxPolicy|6 |Estado de acesso determinado pela Exchange de Caixa de Correio|
|other|7 |Estado de acesso determinado por Exchange|
|compatível|8 |Estado de acesso concedido pelo desafio de conformidade|
|notCompliant|9 |Estado de acesso revogado pelo desafio de conformidade|
|notEnrolled|10 |Estado de acesso revogado pelo desafio de gerenciamento|
|unknownLocation|12 |Estado de acesso devido a localização desconhecida|
|mfaRequired|13 |Estado de acesso devido ao desafio MFA|
|azureADBlockDueToAccessPolicy|14 |Estado de Acesso revogado pela Política de Acesso do AAD|
|compromisedPassword|15 |Estado do Access revogado por senha comprometida|
|deviceNotKnownWithManagedApp|16 |Estado de acesso revogado pelo desafio de aplicativo gerenciado|




