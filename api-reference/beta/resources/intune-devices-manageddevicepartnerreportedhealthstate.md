---
title: tipo de enumeração managedDevicePartnerReportedHealthState
description: Estados de integridade disponíveis para a API de integridade do dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 832e79d759b969dbd96dfd773bac732ec68460d3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528528"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>tipo de enumeração managedDevicePartnerReportedHealthState

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estados de integridade disponíveis para a API de integridade do dispositivo

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|O estado de integridade do dispositivo ainda não foi relatado|
|ativado|1 |O dispositivo foi ativado por um parceiro de defesa contra ameaças móveis, mas ainda não relatou a integridade.|
|desativada|2 |O dispositivo foi desativado por um parceiro de defesa contra ameaças móveis. A integridade do dispositivo não é conhecida.|
|presos|3 |O dispositivo é considerado protegido pelo parceiro de defesa contra ameaças móveis.|
|lowSeverity|4 |O dispositivo é considerado com baixa ameaça pelo parceiro de defesa contra ameaças móveis.|
|mediumSeverity|5 |O dispositivo é considerado como ameaça médio pelo parceiro de defesa contra ameaças móveis.|
|highSeverity|6 |O dispositivo é considerado de alta ameaça pelo parceiro de defesa contra ameaças móveis.|
|Não responde|7 |O dispositivo é considerado sem resposta pelo parceiro de defesa contra ameaças móveis. A integridade do dispositivo não é conhecida.|
|ficasse|8 |O dispositivo é considerado comprometido pelo parceiro de proteção contra ameaças. Isso significa que o dispositivo tem uma ameaça ou risco ativo que não pode ser corrigido facilmente pelo usuário final e o usuário deve entrar em contato com o administrador de ti.|
|configurado incorretamente|9 |O dispositivo é considerado incorretamente configurado com o parceiro de proteção contra ameaças. Isso significa que o dispositivo não tem um perfil ou uma configuração necessária para que o parceiro de defesa contra ameaças funcione corretamente, e, portanto, a análise de ameaças ou riscos não pode ser concluída.|



