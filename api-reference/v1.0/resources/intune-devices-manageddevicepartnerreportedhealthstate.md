---
title: tipo de enumeração managedDevicePartnerReportedHealthState
description: Estados de integridade disponíveis para a API de integridade do dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4e6ef870687f0ee48eebd3d0f8d45eb4c88906ef
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252053"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>tipo de enumeração managedDevicePartnerReportedHealthState

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estados de integridade disponíveis para a API de integridade do dispositivo

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|unknown|,0|O estado de integridade do dispositivo ainda não foi relatado|
|ativado|1|O dispositivo foi ativado por um parceiro de defesa contra ameaças móveis, mas ainda não relatou a integridade.|
|desativada|duas|O dispositivo foi desativado por um parceiro de defesa contra ameaças móveis. A integridade do dispositivo não é conhecida.|
|presos|3D|O dispositivo é considerado protegido pelo parceiro de defesa contra ameaças móveis.|
|lowSeverity|quatro|O dispositivo é considerado com baixa ameaça pelo parceiro de defesa contra ameaças móveis.|
|mediumSeverity|0,5|O dispositivo é considerado como ameaça médio pelo parceiro de defesa contra ameaças móveis.|
|highSeverity|6|O dispositivo é considerado de alta ameaça pelo parceiro de defesa contra ameaças móveis.|
|Não responde|178|O dispositivo é considerado sem resposta pelo parceiro de defesa contra ameaças móveis. A integridade do dispositivo não é conhecida.|
|ficasse|8|O dispositivo é considerado comprometido pelo parceiro de proteção contra ameaças. Isso significa que o dispositivo tem uma ameaça ou risco ativo que não pode ser corrigido facilmente pelo usuário final e o usuário deve entrar em contato com o administrador de ti.|
|configurado incorretamente|241|O dispositivo é considerado incorretamente configurado com o parceiro de proteção contra ameaças. Isso significa que o dispositivo não tem um perfil ou uma configuração necessária para que o parceiro de defesa contra ameaças funcione corretamente, e, portanto, a análise de ameaças ou riscos não pode ser concluída.|



