---
title: tipo de enumeração configurationManagerClientState
description: Estado do cliente de gerenciador de configurações
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bfcfeb826ce679b281e74a6c320ab737f0f1a969
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060626"
---
# <a name="configurationmanagerclientstate-enum-type"></a>tipo de enumeração configurationManagerClientState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado do cliente de gerenciador de configurações

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|O agente do Gerenciador de configurações é mais antigo que 1806 ou não instalado ou este dispositivo não foi verificado no Intune por mais de 30 dias.|
|instalação|1 |O agente do Gerenciador de configurações está instalado, mas talvez ainda não esteja aparecendo no console do Gerenciador de configurações. Aguarde algumas horas para que ele seja atualizado.|
|condições|7 |Este dispositivo pôde fazer check-in com o serviço do Gerenciador de configurações com êxito.|
|installFailed|8 |Falha ao instalar o agente do Gerenciador de configurações.|
|updateFailed|11 |A atualização da versão x para a versão y do agente do Gerenciador de configuração falhou. |
|communicationError|19|O agente do Gerenciador de configurações pôde acessar o serviço do Configuration Manager no passado, mas agora não é mais possível. |






