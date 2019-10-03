---
title: tipo de enumeração deviceEnrollmentType
description: Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ae60fd6657cf902eb5bdd0f919d446527b00d9a9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368271"
---
# <a name="deviceenrollmenttype-enum-type"></a>tipo de enumeração deviceEnrollmentType

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




