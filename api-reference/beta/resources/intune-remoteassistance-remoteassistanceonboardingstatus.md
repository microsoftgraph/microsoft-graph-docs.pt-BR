---
title: tipo de enumeração remoteAssistanceOnboardingStatus
description: O status atual do conector do TeamViewer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ccb04964c7608c24ec8822bac7832aaf77bdfd7f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287785"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a>tipo de enumeração remoteAssistanceOnboardingStatus

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O status atual do conector do TeamViewer

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notOnboarded|,0|O status relatado quando não há conector do TeamViewer ativo configurado ou ativo|
|integração|1|O status relatado quando o sistema iniciou uma conexão do TeamViewer, mas o serviço ainda não concluiu a confirmação de um conector|
|integrado|duas|O status relatado quando o sistema trocava com êxito informações de conta com o TeamViewer e agora pode iniciar sessões de assistência remota com clientes|




