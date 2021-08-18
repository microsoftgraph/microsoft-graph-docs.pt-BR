---
title: tipo de número managementAgentType
description: Tipo de agente de gerenciamento.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a157111db947e9e7c186c30be6cc63a709b82922
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58263307"
---
# <a name="managementagenttype-enum-type"></a>tipo de número managementAgentType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de agente de gerenciamento.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|eas|1 |O dispositivo é gerenciado por Exchange servidor.|
|mdm|2|O dispositivo é gerenciado pelo MDM do Intune.|
|easMdm|3 |O dispositivo é gerenciado pelo servidor Exchange e pelo MDM do Intune.|
|intuneClient|4 |Cliente do Intune gerenciado.|
|easIntuneClient|5 |O dispositivo é gerenciado duplo do cliente EAS e do Intune.|
|configurationManagerClient|8 |O dispositivo é gerenciado pelo Configuration Manager.|
|configurationManagerClientMdm|10 |O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.|
|configurationManagerClientMdmEas|11 |O dispositivo é gerenciado pelo Configuration Manager, MDM e Eas.|
|desconhecido|16 |Tipo de agente de gerenciamento desconhecido.|
|jamf|32|Os atributos do dispositivo são buscados do Jamf.|
|googleCloudDevicePolicyController|64|O dispositivo é gerenciado pelo CloudDPC do Google.|
|microsoft365ManagedMdm|258|Esse dispositivo é gerenciado por Microsoft 365 através do Intune.|
|msSense|1024|Ainda não documentado|
|intuneAosp|2048|Esse dispositivo é gerenciado pelo MDM do Intune para dispositivos AOSP (Android Open Source Project)|




