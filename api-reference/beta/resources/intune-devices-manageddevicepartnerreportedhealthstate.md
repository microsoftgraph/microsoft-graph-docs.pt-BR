---
title: tipo de enumeração managedDevicePartnerReportedHealthState
description: Estados de integridade disponíveis para a API de integridade do dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8935c5715c9248b7c50f87d8835979906a7b3801
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999756"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>tipo de enumeração managedDevicePartnerReportedHealthState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estados de integridade disponíveis para a API de integridade do dispositivo

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|O estado de integridade do dispositivo ainda não foi relatado|
|ativado|1|O dispositivo foi ativado por um parceiro de defesa contra ameaças móveis, mas ainda não relatou a integridade.|
|desativada|duas|O dispositivo foi desativado por um parceiro de defesa contra ameaças móveis. A integridade do dispositivo não é conhecida.|
|presos|3D|O dispositivo é considerado protegido pelo parceiro de defesa contra ameaças móveis.|
|lowSeverity|quatro|O dispositivo é considerado com baixa ameaça pelo parceiro de defesa contra ameaças móveis.|
|mediumSeverity|0,5|O dispositivo é considerado como ameaça médio pelo parceiro de defesa contra ameaças móveis.|
|highSeverity|6|O dispositivo é considerado de alta ameaça pelo parceiro de defesa contra ameaças móveis.|
|Não responde|178|O dispositivo é considerado sem resposta pelo parceiro de defesa contra ameaças móveis. A integridade do dispositivo não é conhecida.|
|ficasse|8 |O dispositivo é considerado comprometido pelo parceiro de proteção contra ameaças. Isso significa que o dispositivo tem uma ameaça ou risco ativo que não pode ser corrigido facilmente pelo usuário final e o usuário deve entrar em contato com o administrador de ti.|
|configurado incorretamente|9 |O dispositivo é considerado incorretamente configurado com o parceiro de proteção contra ameaças. Isso significa que o dispositivo não tem um perfil ou uma configuração necessária para que o parceiro de defesa contra ameaças funcione corretamente, e, portanto, a análise de ameaças ou riscos não pode ser concluída.|





