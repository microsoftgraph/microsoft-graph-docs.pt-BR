---
title: tipo de enumeração deviceEnrollmentType
description: Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c0e75b3a8ab7cc9ebf3929c0764eba243cb1357c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49306867"
---
# <a name="deviceenrollmenttype-enum-type"></a>tipo de enumeração deviceEnrollmentType

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|O valor padrão, o tipo de registro não foi coletado.|
|userregistrar|1|Registro controlado pelo usuário por meio do canal BYOD.|
|deviceEnrollmentManager|duas|Registro de usuário com uma conta de Gerenciador de registro de dispositivo.|
|appleBulkWithUser|3D|Inscrição em massa da Apple com o desafio do usuário. (DEP, Apple Configurator)|
|appleBulkWithoutUser|4 |Inscrição em massa da Apple sem o desafio do usuário. (DEP, Apple Configurator, configuração móvel)|
|windowsAzureADJoin|5 |Ingressar no Azure AD do Windows 10.|
|windowsBulkUserless|6 |Registro em massa do Windows 10 através do ICD com o certificado.|
|windowsAutoEnrollment|7 |Registro automático do Windows 10. (Adicionar conta de trabalho)|
|windowsBulkAzureDomainJoin|8 |Ingresso no Azure AD em massa do Windows 10.|
|windowsCoManagement|9 |Windows 10 Co-Management disparado por AutoPilot ou política de grupo.|
|appleUserEnrollment|11 |Dispositivo gerenciado pelo registro de usuário da Apple|
|appleUserEnrollmentWithServiceAccount|12 |Dispositivo gerenciado pelo registro de usuário da Apple com conta de serviço|
|azureAdJoinUsingAzureVmExtension|14 |Azure AD ingressar no registro quando uma máquina virtual do Azure é provisionada|
|androidEnterpriseDedicatedDevice|15 |Dispositivo dedicado corporativo Android|
|androidEnterpriseFullyManaged|16 |Android Enterprise totalmente gerenciado|
|androidEnterpriseCorporateWorkProfile|17 |Perfil de trabalho corporativo do Android Enterprise|




