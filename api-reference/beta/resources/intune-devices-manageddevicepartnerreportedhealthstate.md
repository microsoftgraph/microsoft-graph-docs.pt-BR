---
title: tipo de enum managedDevicePartnerReportedHealthState
description: Estados de integridade disponíveis para a API de integridade do dispositivo
author: tfitzmac
ms.openlocfilehash: 41dcc927e85664acf28c7cc654fa01d00d1e4b52
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321025"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>tipo de enum managedDevicePartnerReportedHealthState

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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





