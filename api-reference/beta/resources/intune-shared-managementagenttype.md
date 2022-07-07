---
title: Tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a157111db947e9e7c186c30be6cc63a709b82922
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671541"
---
# <a name="managementagenttype-enum-type"></a>Tipo de enumeração managementAgentType

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

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
|microsoft365ManagedMdm|258|Esse dispositivo é gerenciado pelo Microsoft 365 por meio Intune.|
|msSense|1024|Ainda não documentado|
|intuneAosp|2048|Esse dispositivo é gerenciado pelo MDM do Intune para dispositivos AOSP (Projeto de Software Livre Android)|




