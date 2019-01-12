---
title: tipo de enum deviceEnrollmentType
description: Maneiras possíveis de adição de um dispositivo móvel gerenciamento.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bffe0e592240cbeee22a63dac8c339a0d3b3ff3d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946835"
---
# <a name="deviceenrollmenttype-enum-type"></a>tipo de enum deviceEnrollmentType

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Maneiras possíveis de adição de um dispositivo móvel gerenciamento.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|unknown|0|O valor padrão, tipo de registro não foi coletado.|
|userEnrollment|1|Inscrição do orientado por usuário por meio do canal BYOD.|
|deviceEnrollmentManager|2|Inscrição do usuário com uma conta de Gerenciador de inscrição do dispositivo.|
|appleBulkWithUser|3|Inscrição do Apple em massa com o desafio de usuário. Configurador Apple (DEP)|
|appleBulkWithoutUser|4|Inscrição do Apple em massa sem o desafio de usuário. (DEP, Apple configurador, móvel Config)|
|windowsAzureADJoin|5|Windows Azure AD de 10 ingressam.|
|windowsBulkUserless|6|Inscrição em massa de 10 Windows por meio de ICD com certificado.|
|windowsAutoEnrollment|7|Inscrição automática do Windows 10. (Adicionar a conta do trabalho)|
|windowsBulkAzureDomainJoin|8|Windows 10 em massa ingressar do Windows Azure AD.|
|windowsCoManagement|9|Gerenciamento de colegas de 10 Windows acionadas por piloto automático ou a diretiva de grupo.|





