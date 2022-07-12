---
title: Tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8e178c22a13e089b89b709757f38d9abb3cc04df
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66731929"
---
# <a name="managementagenttype-enum-type"></a>Tipo de enumeração managementAgentType

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de agente de gerenciamento.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Eas|1|O dispositivo é gerenciado pelo exchange server.|
|Mdm|2|O dispositivo é gerenciado por Intune MDM.|
|easMdm|3|O dispositivo é gerenciado pelo servidor Exchange e Intune MDM.|
|intuneClient|4|Intune cliente gerenciado.|
|easIntuneClient|5|O dispositivo é EAS e Intune cliente dual gerenciado.|
|configurationManagerClient|8 |O dispositivo é gerenciado por Configuration Manager.|
|configurationManagerClientMdm|10|O dispositivo é gerenciado por Configuration Manager e MDM.|
|configurationManagerClientMdmEas|11|O dispositivo é gerenciado por Configuration Manager, MDM e Eas.|
|desconhecido|16|Tipo de agente de gerenciamento desconhecido.|
|jamf|32|Os atributos de dispositivo são buscados no Jamf.|
|googleCloudDevicePolicyController|64|O dispositivo é gerenciado pelo CloudDPC do Google.|





