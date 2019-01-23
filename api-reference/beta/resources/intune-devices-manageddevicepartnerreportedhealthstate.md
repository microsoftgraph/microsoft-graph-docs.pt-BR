---
title: tipo de enum managedDevicePartnerReportedHealthState
description: Estados de integridade disponíveis para a API de integridade do dispositivo
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cb5b13ceceab27e1e88a69310a3198159f5e24c1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418824"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>tipo de enum managedDevicePartnerReportedHealthState

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Estados de integridade disponíveis para a API de integridade do dispositivo

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|unknown|0|Estado de integridade do dispositivo ainda não é relatado|
|ativado|1|Dispositivo tiver sido ativado por um parceiro de defesa contra ameaças móveis, mas ainda não tiver relatado integridade.|
|desativado|2|Dispositivo foi desativado por um parceiro de defesa contra ameaças móveis. A integridade do dispositivo não é conhecida.|
|protegido|3|Dispositivo é considerado protegido pelo parceiro defesa contra ameaças móveis.|
|lowSeverity|4|Dispositivo é considerado ameaça baixa pelo parceiro defesa contra ameaças móveis.|
|mediumSeverity|5|Dispositivo é considerado ameaça média pelo parceiro defesa contra ameaças móveis.|
|highSeverity|6|Dispositivo é considerado alta ameaça pelo parceiro defesa contra ameaças móveis.|
|não responde|7|Dispositivo é considerado não responde pelo parceiro defesa contra ameaças móveis. A integridade do dispositivo não é conhecida.|
|comprometida|8|Dispositivo é considerado comprometida pelo parceiro defesa contra ameaças. Isso significa que o dispositivo tem uma ameaça ativo ou o risco que não pode ser facilmente remediado pelo usuário final e o usuário deve entre em contato com seu administrador de TI.|
|definida incorretamente|9|Dispositivo é considerado definida incorretamente com o parceiro de defesa contra ameaças. Isso significa que o dispositivo está faltando um perfil necessária ou a configuração do parceiro de defesa de ameaça funcione corretamente e é assim ameaça ou a análise de riscos não é possível concluir.|




