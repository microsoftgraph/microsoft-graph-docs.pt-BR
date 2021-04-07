---
title: Tipo de número deviceEnrollmentType
description: Possíveis maneiras de adicionar um dispositivo móvel ao gerenciamento.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3d3bc9b0862dd376b393019838980ce9c82c7df3
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612115"
---
# <a name="deviceenrollmenttype-enum-type"></a>Tipo de número deviceEnrollmentType

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Possíveis maneiras de adicionar um dispositivo móvel ao gerenciamento.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Valor padrão, tipo de registro não coletado.|
|userEnrollment|1|Registro orientado pelo usuário por meio do canal BYOD.|
|deviceEnrollmentManager|2|Registro de usuário com uma conta do gerenciador de registro de dispositivo.|
|appleBulkWithUser|3|Registro em massa da Apple com desafio do usuário. (DEP, Apple Configurator)|
|appleBulkWithoutUser|4 |Registro em massa da Apple sem desafio do usuário. (DEP, Apple Configurator, Mobile Config)|
|windowsAzureADJoin|5 |Ingressar no Windows 10 Azure AD.|
|windowsBulkUserless|6 |Registro em massa do Windows 10 por meio do ICD com certificado.|
|windowsAutoEnrollment|7 |Registro automático do Windows 10. (Adicionar conta de trabalho)|
|windowsBulkAzureDomainJoin|8 |Ingressar no Azure AD em massa do Windows 10.|
|windowsCoManagement|9 |O Windows 10 Co-Management acionado pelo AutoPilot ou Pela Política de Grupo.|
|windowsAzureADJoinUsingDeviceAuth|10 |Ingressar no Windows 10 Azure AD usando o Device Auth.|
|appleUserEnrollment|11|Dispositivo gerenciado pelo registro de usuário da Apple|
|appleUserEnrollmentWithServiceAccount|12 |Dispositivo gerenciado pelo registro de usuário da Apple com conta de serviço|
|azureAdJoinUsingAzureVmExtension|14 |Registro de participação do Azure AD quando uma VM do Azure é provisionada|
|androidEnterpriseDedicatedDevice|15 |Dispositivo dedicado do Android Enterprise|
|androidEnterpriseFullyManaged|16 |Android Enterprise Totalmente Gerenciado|
|androidEnterpriseCorporateWorkProfile|17 |Perfil de Trabalho Corporativo do Android Enterprise|




