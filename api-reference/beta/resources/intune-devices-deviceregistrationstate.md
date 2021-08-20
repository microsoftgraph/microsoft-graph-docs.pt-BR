---
title: Tipo de número deviceRegistrationState
description: Status do registro do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7197e541b46cc3f63340ee804f126a14d862283c616a1baf980c81725e6b5a87
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54197979"
---
# <a name="deviceregistrationstate-enum-type"></a>Tipo de número deviceRegistrationState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Status do registro do dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notRegistered|0|O dispositivo não está registrado.|
|registered|2|O dispositivo está registrado.|
|revogado|3 |O dispositivo foi bloqueado, apagado ou retirado.|
|keyConflict|4 |O dispositivo tem um conflito chave.|
|approvalPending|5 |O dispositivo está aguardando aprovação.|
|certificateReset|6 |O certificado do dispositivo foi redefinido.|
|notRegisteredPendingEnrollment|7 |O dispositivo não está registrado e o registro pendente.|
|desconhecido|8 |O status do registro do dispositivo é desconhecido.|




