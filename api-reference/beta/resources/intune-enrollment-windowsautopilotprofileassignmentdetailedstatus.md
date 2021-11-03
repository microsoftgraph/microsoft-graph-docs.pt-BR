---
title: tipo de número windowsAutopilotProfileAssignmentDetailedStatus
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bd81c03006349bf3401c736c092dbab25e7ca0ac
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696305"
---
# <a name="windowsautopilotprofileassignmentdetailedstatus-enum-type"></a>tipo de número windowsAutopilotProfileAssignmentDetailedStatus

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|0|Nenhum status detalhado de atribuição|
|hardwareRequirementsNotMet|1|Os requisitos de hardware não são atendidos. Isso pode acontecer se um Perfil autopiloto de implantação for atribuído a um dispositivo sem TPM 2.0.|
|surfaceHubProfileNotSupported|2|Indica que um perfil Surface Hub AutoPilot é atribuído a um dispositivo que não Surface Hub(Aruba).|
|holoLensProfileNotSupported|3|Indica que um perfil HoloLens AutoPilot é atribuído a um dispositivo que não HoloLens.|
|windowsPcProfileNotSupported|4|Indica que um perfil Windows autoPilot do computador é atribuído a um dispositivo que não Windows computador.|
|surfaceHub2SProfileNotSupported|5|Indica que um perfil do Surface Hub 2S AutoPilot é atribuído a um dispositivo que não é o Surface Hub 2S.|
|unknownFutureValue|99|Espaço reservado para um número evolvável, mas esse número nunca é retornado ao chamador, portanto, não deve ser necessário.|



