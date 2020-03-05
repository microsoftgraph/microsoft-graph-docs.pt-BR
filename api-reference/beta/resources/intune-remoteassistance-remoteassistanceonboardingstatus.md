---
title: tipo de enumeração remoteAssistanceOnboardingStatus
description: O status atual do conector do TeamViewer
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 64b8e1f1735890236aed6a9f642d4fa5860e016b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527524"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a>tipo de enumeração remoteAssistanceOnboardingStatus

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O status atual do conector do TeamViewer

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notOnboarded|,0|O status relatado quando não há conector do TeamViewer ativo configurado ou ativo|
|integração|1 |O status relatado quando o sistema iniciou uma conexão do TeamViewer, mas o serviço ainda não concluiu a confirmação de um conector|
|integrado|2 |O status relatado quando o sistema trocava com êxito informações de conta com o TeamViewer e agora pode iniciar sessões de assistência remota com clientes|



