---
title: tipo de enum deviceEnrollmentType
description: Maneiras possíveis de adição de um dispositivo móvel gerenciamento.
author: tfitzmac
ms.openlocfilehash: 88135947f882433a35fa518b750274f38f48dcc1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329600"
---
# <a name="deviceenrollmenttype-enum-type"></a>tipo de enum deviceEnrollmentType

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Maneiras possíveis de adição de um dispositivo móvel gerenciamento.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|unknown|0|O valor padrão, tipo de registro não foi coletado.|
|userEnrollment|1|Inscrição do orientado por usuário por meio do canal BYOD.|
|deviceEnrollmentManager|2|Inscrição do usuário com uma conta de Gerenciador de inscrição do dispositivo.|
|appleBulkWithUser|3|Inscrição do Apple em massa com o desafio de usuário (DEP, Apple configurador).|
|appleBulkWithoutUser|4|Inscrição do Apple em massa sem o desafio de usuário (DEP, Apple configurador, Mobile Config).|
|windowsAzureADJoin|5|Windows Azure AD de 10 ingressam.|
|windowsBulkUserless|6|Inscrição em massa de 10 Windows por meio de ICD com certificado.|
|windowsAutoEnrollment|7|Inscrição automática do Windows 10. (Adicionar a conta do trabalho)|
|windowsBulkAzureDomainJoin|8|Windows 10 em massa ingressar do Windows Azure AD.|
|windowsCoManagement|9|Gerenciamento de colegas Windows 10 acionado por piloto automático ou a diretiva de grupo.|



