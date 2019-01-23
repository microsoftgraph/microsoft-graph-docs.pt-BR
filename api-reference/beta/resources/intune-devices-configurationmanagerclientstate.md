---
title: tipo de enum configurationManagerClientState
description: Estado de cliente do Gerenciador de configuração
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 82f4b677001346f9bd32c1bc54bed6e7fbac253d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425782"
---
# <a name="configurationmanagerclientstate-enum-type"></a>tipo de enum configurationManagerClientState

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

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




