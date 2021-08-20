---
title: tipo denum configurationManagerClientState
description: Estado do cliente de gerenciador de configurações
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3bcac417f0a0a156a998bd65a50a6baf9697b801a3c8484398fc57ad59fc3f53
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251285"
---
# <a name="configurationmanagerclientstate-enum-type"></a>tipo denum configurationManagerClientState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado do cliente de gerenciador de configurações

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|O agente do gerenciador de configuração tem mais de 1806 ou não foi instalado ou esse dispositivo não fez check-in no Intune por mais de 30 dias.|
|instalado|1 |O agente do gerenciador de configuração está instalado, mas pode não estar aparecendo no console do gerenciador de configuração ainda. Aguarde algumas horas para atualizar.|
|healthy|7 |Esse dispositivo foi capaz de fazer check-in com o serviço de gerenciador de configuração com êxito.|
|installFailed|8 |O agente do gerenciador de configuração falhou na instalação.|
|updateFailed|11 |A atualização da versão x para a versão y do agente do gerenciador de configuração falhou. |
|communicationError|19|O agente do gerenciador de configuração foi capaz de alcançar o serviço de gerenciador de configuração no passado, mas agora não é mais capaz de. |




