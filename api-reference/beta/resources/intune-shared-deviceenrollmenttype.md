---
title: tipo de enumeração deviceEnrollmentType
description: Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a9c5c5fbdd68af1c78e55fc023a8c85642928889
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940012"
---
# <a name="deviceenrollmenttype-enum-type"></a>tipo de enumeração deviceEnrollmentType

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|O valor padrão, o tipo de registro não foi coletado.|
|userregistrar|1|Registro controlado pelo usuário por meio do canal BYOD.|
|deviceEnrollmentManager|duas|Registro de usuário com uma conta de Gerenciador de registro de dispositivo.|
|appleBulkWithUser|3D|Inscrição em massa da Apple com o desafio do usuário. (DEP, Apple Configurator)|
|appleBulkWithoutUser|quatro|Inscrição em massa da Apple sem o desafio do usuário. (DEP, Apple Configurator, configuração móvel)|
|windowsAzureADJoin|0,5|Ingressar no Azure AD do Windows 10.|
|windowsBulkUserless|6|Registro em massa do Windows 10 através do ICD com o certificado.|
|windowsAutoEnrollment|178|Registro automático do Windows 10. (Adicionar conta de trabalho)|
|windowsBulkAzureDomainJoin|8 |Ingresso no Azure AD em massa do Windows 10.|
|windowsCoManagement|9 |Co-gerenciamento de intergestão do Windows 10 disparado por AutoPilot ou política de grupo.|




