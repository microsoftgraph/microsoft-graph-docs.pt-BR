---
title: Tipo de número deviceEnrollmentType
description: Possíveis maneiras de adicionar um dispositivo móvel ao gerenciamento.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e45ddd00b11ced1a406d03e8339055ebda1cd82e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59051031"
---
# <a name="deviceenrollmenttype-enum-type"></a>Tipo de número deviceEnrollmentType

Namespace: microsoft.graph

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
|windowsAzureADJoin|5 |Windows 10 Ingressar no Azure AD.|
|windowsBulkUserless|6 |Windows 10 Registro em massa por meio do ICD com certificado.|
|windowsAutoEnrollment|7 |Windows 10 registro automático. (Adicionar conta de trabalho)|
|windowsBulkAzureDomainJoin|8 |Windows 10 participar em massa do Azure AD.|
|windowsCoManagement|9 |Windows 10 Co-Management acionado pelo AutoPilot ou Pela Política de Grupo.|
|windowsAzureADJoinUsingDeviceAuth|10 |Windows 10 Ingressar no Azure AD usando Device Auth.|
|appleUserEnrollment|11|Dispositivo gerenciado pelo registro de usuário da Apple|
|appleUserEnrollmentWithServiceAccount|12 |Dispositivo gerenciado pelo registro de usuário da Apple com conta de serviço|
|azureAdJoinUsingAzureVmExtension|14 |Registro de participação do Azure AD quando uma VM do Azure é provisionada|
|androidEnterpriseDedicatedDevice|15 |Dispositivo Enterprise Android dedicado|
|androidEnterpriseFullyManaged|16 |Android Enterprise Totalmente Gerenciado|
|androidEnterpriseCorporateWorkProfile|17 |Perfil Enterprise trabalho corporativo do Android|




