---
title: Tipo de número deviceRegistrationState
description: Status do registro do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 032b4bcdc6b84df6d02fccde5e64b16a0d1dd92b
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60447372"
---
# <a name="deviceregistrationstate-enum-type"></a>Tipo de número deviceRegistrationState

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Status do registro do dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notRegistered|0|O dispositivo não está registrado.|
|registered|2|O dispositivo está registrado.|
|revogado|3|O dispositivo foi bloqueado, apagado ou retirado.|
|keyConflict|4 |O dispositivo tem um conflito chave.|
|approvalPending|5|O dispositivo está aguardando aprovação.|
|certificateReset|6 |O certificado do dispositivo foi redefinido.|
|notRegisteredPendingEnrollment|7 |O dispositivo não está registrado e o registro pendente.|
|desconhecido|8 |O status do registro do dispositivo é desconhecido.|



