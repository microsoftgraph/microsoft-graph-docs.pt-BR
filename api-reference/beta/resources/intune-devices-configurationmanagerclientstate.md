---
title: tipo de enum configurationManagerClientState
description: Estado de cliente do Gerenciador de configuração
author: tfitzmac
ms.openlocfilehash: dc67a5fb1c517e65da937996ed65adaa621fa3c5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354044"
---
# <a name="configurationmanagerclientstate-enum-type"></a>tipo de enum configurationManagerClientState

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Estado de cliente do Gerenciador de configuração
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|unknown|0|Agente do Gerenciador de configuração é mais antigo que 1806 ou não está instalado ou este dispositivo não tiver verificado em Intune por mais de 30 dias.|
|instalado|1|O agente do Gerenciador de configuração está instalado, mas pode não ser aparecendo no console do configuration manager ainda. Aguarde algumas horas para que ele seja atualizada.|
|Íntegro|7|Este dispositivo foi capaz de check-in com o serviço do Gerenciador de configuração com êxito.|
|installFailed|8|Falha na instalação do agente do Gerenciador de configuração.|
|updateFailed|11|Falha na atualização da versão x a y da versão do agente do Gerenciador de configuração. |
|communicationError|19|O agente do Gerenciador de configuração foi capaz de acessar o serviço do Gerenciador de configuração no passado, mas agora não é mais possível. |





