---
title: tipo de enumeração deviceEnrollmentType
description: Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b186110c4f69ea7b6f4d12c9fb2a333927f81385
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173651"
---
# <a name="deviceenrollmenttype-enum-type"></a>tipo de enumeração deviceEnrollmentType

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|unknown|,0|O valor padrão, o tipo de registro não foi coletado.|
|userRegistrar|1|Registro controlado pelo usuário por meio do canal BYOD.|
|deviceEnrollmentManager|duas|Registro de usuário com uma conta de Gerenciador de registro de dispositivo.|
|appleBulkWithUser|3D|Inscrição em massa da Apple com o desafio do usuário. (DEP, Apple conFigurator)|
|appleBulkWithoutUser|quatro|Inscrição em massa da Apple sem o desafio do usuário. (DEP, Apple conFigurator, configuração móvel)|
|windowsAzureADJoin|0,5|Ingressar no Azure AD do Windows 10.|
|windowsBulkUserless|6|Registro em massa do Windows 10 através do ICD com o certificado.|
|windowsAutoEnrollment|178|Registro automático do Windows 10. (Adicionar conta de trabalho)|
|windowsBulkAzureDomainJoin|8|Ingresso no Azure AD em massa do Windows 10.|
|windowsCoManagement|241|Co-gerenciamento de interGestão do Windows 10 disparado por autoPilot ou política de grupo.|




