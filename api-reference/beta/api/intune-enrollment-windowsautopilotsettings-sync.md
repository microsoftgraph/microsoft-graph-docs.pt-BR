---
title: ação sync
description: Inicia uma sincronização de todos os dispositivos registrados do AutoPilot da Store para Empresas e de outros portais. Se a sincronização for bem-sucedida, essa ação retornará um código de resposta 204 No Content. Se uma sincronização já estiver em andamento, a ação retornará um código de resposta conflict 409.  Se essa ação de sincronização for chamada dentro de 10 minutos da sincronização anterior, a ação retornará um código de resposta 429 Solicitações Demais.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 298d3a41a8d8e5fcfcbb2355109226e1af562511765578446946b0c84c5b12b4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54204090"
---
# <a name="sync-action"></a>Ação sync

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Inicia uma sincronização de todos os dispositivos registrados do AutoPilot da Store para Empresas e de outros portais. Se a sincronização for bem-sucedida, essa ação retornará um código de resposta 204 No Content. Se uma sincronização já estiver em andamento, a ação retornará um código de resposta conflict 409.  Se essa ação de sincronização for chamada dentro de 10 minutos da sincronização anterior, a ação retornará um código de resposta 429 Solicitações Demais.

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotSettings/sync
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings/sync
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 204 No Content
```




