---
title: Tipo de enumeração deviceEnrollmentType
description: Possíveis maneiras de adicionar um dispositivo móvel ao gerenciamento.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a53c4fadbce9703e4e68b54a86cfff80e1bd3944
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735366"
---
# <a name="deviceenrollmenttype-enum-type"></a>Tipo de enumeração deviceEnrollmentType

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Possíveis maneiras de adicionar um dispositivo móvel ao gerenciamento.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Valor padrão, tipo de registro não coletado.|
|userEnrollment|1|Registro controlado pelo usuário por meio do canal BYOD.|
|deviceEnrollmentManager|2|Registro de usuário com uma conta do gerenciador de registro de dispositivo.|
|appleBulkWithUser|3|Registro em massa da Apple com desafio do usuário. (DEP, Apple Configurator)|
|appleBulkWithoutUser|4|Registro em massa da Apple sem desafio do usuário. (DEP, Apple Configurator, Configuração Móvel)|
|windowsAzureADJoin|5|Windows 10 Azure AD ingressar.|
|windowsBulkUserless|6 |Windows 10 registro em massa por meio do ICD com certificado.|
|windowsAutoEnrollment|7 |Windows 10 registro automático. (Adicionar conta corporativa)|
|windowsBulkAzureDomainJoin|8 |Windows 10 em massa Azure AD Join.|
|windowsCoManagement|9 |Windows 10 Co-Management acionado pelo AutoPilot ou Política de Grupo.|
|windowsAzureADJoinUsingDeviceAuth|10|Windows 10 Azure AD ingressar usando a Autenticação de Dispositivo.|
|appleUserEnrollment|11|Dispositivo gerenciado pelo registro de usuário da Apple|
|appleUserEnrollmentWithServiceAccount|12 |Dispositivo gerenciado pelo registro de usuário da Apple com conta de serviço|





