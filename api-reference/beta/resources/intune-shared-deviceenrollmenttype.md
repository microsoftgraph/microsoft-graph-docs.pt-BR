---
title: tipo de enum deviceEnrollmentType
description: Maneiras possíveis de adição de um dispositivo móvel gerenciamento.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aed1f40604a765b1a434bca35dbb356e65e8ccd5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399287"
---
# <a name="deviceenrollmenttype-enum-type"></a>tipo de enum deviceEnrollmentType

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

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




