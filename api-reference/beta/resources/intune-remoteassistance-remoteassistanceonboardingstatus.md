---
title: tipo de enumeração remoteAssistanceOnboardingStatus
description: O status atual do conector do TeamViewer
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 23490e61f4134b723cfc066043f132c44c295019
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787894"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a>tipo de enumeração remoteAssistanceOnboardingStatus

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O status atual do conector do TeamViewer

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notOnboarded|,0|O status relatado quando não há conector do TeamViewer ativo configurado ou ativo|
|integração|1|O status relatado quando o sistema iniciou uma conexão do TeamViewer, mas o serviço ainda não concluiu a confirmação de um conector|
|integrado|duas|O status relatado quando o sistema trocava com êxito informações de conta com o TeamViewer e agora pode iniciar sessões de assistência remota com clientes|





