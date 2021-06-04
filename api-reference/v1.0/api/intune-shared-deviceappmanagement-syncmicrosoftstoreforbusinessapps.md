---
title: Ação syncMicrosoftStoreForBusinessApps
description: Sincroniza a conta do Intune com o Microsoft Store For Business
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7a9deb0ab2e84a4debf11040010bc65fad01f65b
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732320"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a>Ação syncMicrosoftStoreForBusinessApps

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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

O objeto de resposta mostrado aqui pode ser truncado para brevidade. Todas as propriedades serão retornadas de uma chamada real.

``` http
HTTP/1.1 204 No Content
```









