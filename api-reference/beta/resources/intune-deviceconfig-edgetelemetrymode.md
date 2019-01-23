---
title: tipo de enum edgeTelemetryMode
description: Tipo de dados enviados à Microsoft 365 análise de navegação
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 81d429f7629a5d6a6f2593785605902065d9f1c7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429120"
---
# <a name="edgetelemetrymode-enum-type"></a>tipo de enum edgeTelemetryMode

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Tipo de dados enviados à Microsoft 365 análise de navegação

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|não-configuradas|0|Padrão – sem dados de telemetria coletados ou enviados|
|intranet|1|Permitir envio somente histórico de intranet: somente enviar dados para sites de intranet do histórico de navegação|
|Internet|2|Permitem o envio somente histórico de internet: enviar apenas procurando dados de histórico para sites da internet|
|intranetAndInternet|3|Permitem o envio de histórico de intranet quanto da internet: envio procurando dados de histórico para sites de intranet e internet|




