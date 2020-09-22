---
title: tipo de enumeração deviceRegistrationState
description: Status do registro do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 628d4c6c253349e54747d4fce836a2b4c8f4579f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081423"
---
# <a name="deviceregistrationstate-enum-type"></a>tipo de enumeração deviceRegistrationState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Status do registro do dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Não registrado|,0|O dispositivo não está registrado.|
|inscreve|2 |O dispositivo está registrado.|
|revogado|3D|O dispositivo foi bloqueado, apagado ou desativado.|
|keyconflict|4 |O dispositivo tem um conflito de teclas.|
|approvalPending|5 |O dispositivo está aguardando aprovação.|
|certificateReset|6 |O certificado de dispositivo foi redefinido.|
|notRegisteredPendingEnrollment|7 |O dispositivo não está registrado e registro pendente.|
|desconhecido|8 |O status do registro do dispositivo é desconhecido.|






