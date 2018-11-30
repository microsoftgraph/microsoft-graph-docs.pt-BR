---
title: tipo de enum habilitação
description: 'Valores usados para indicar o status de um dispositivo. '
ms.openlocfilehash: 5e72df98d33a7d3502dae4bc369781b69bc6aeb0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036767"
---
# <a name="enablement-enum-type"></a>tipo de enum habilitação

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores usados para indicar o status de um dispositivo. 

Observe que há uma diferença entre desabilitado e não configurado.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|não-configuradas|0|Valor de padrão de dispositivo, sem intenção.|
|enabled|1|Permite a configuração no dispositivo.|
|desabilitado|2|Desativa a configuração no dispositivo.|
