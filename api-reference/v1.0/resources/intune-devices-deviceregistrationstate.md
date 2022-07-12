---
title: Tipo de enumeração deviceRegistrationState
description: Status de registro do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a104fb6f347d24dbb2e3d373a1046148486b387e
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730634"
---
# <a name="deviceregistrationstate-enum-type"></a>Tipo de enumeração deviceRegistrationState

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Status de registro do dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notRegistered|0|O dispositivo não está registrado.|
|Registrado|2|O dispositivo está registrado.|
|Revogada|3|O dispositivo foi bloqueado, apagado ou desativado.|
|keyConflict|4|O dispositivo tem um conflito de chave.|
|approvalPending|5|O dispositivo está com aprovação pendente.|
|certificateReset|6 |O certificado do dispositivo foi redefinido.|
|notRegisteredPendingEnrollment|7 |O dispositivo não está registrado e o registro está pendente.|
|desconhecido|8 |O status de registro do dispositivo é desconhecido.|





