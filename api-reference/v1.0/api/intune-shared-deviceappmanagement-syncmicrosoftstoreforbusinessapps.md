---
title: Ação syncMicrosoftStoreForBusinessApps
description: Sincroniza a conta do Intune com o Microsoft Store For Business
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f485349a2bcf9b69eee428e98be39bce7bb5f50f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361564"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a>Ação syncMicrosoftStoreForBusinessApps

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Sincroniza a conta do Intune com o Microsoft Store For Business

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)| 
| &nbsp; &nbsp; _Integração_ | DeviceManagementApps.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
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

## <a name="example-request"></a>Exemplo de solicitação

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a>Resposta

O objeto de resposta mostrado aqui pode estar truncado por brevidade. Todas as propriedades serão retornadas de uma chamada real.

``` http
HTTP/1.1 204 No Content
```




