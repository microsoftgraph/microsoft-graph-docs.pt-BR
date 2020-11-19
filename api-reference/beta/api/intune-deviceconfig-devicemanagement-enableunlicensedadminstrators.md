---
title: ação enableUnlicensedAdminstrators
description: Após a habilitação, os usuários atribuídos como administradores por meio de associações de atribuição de função não precisarão mais de uma licença do Intune atribuída. Você está limitado a 350 membros diretos não licenciados para cada grupo de segurança do AAD em uma atribuição de função, mas você pode atribuir vários grupos de segurança do AAD a uma função se precisar dar suporte a mais de 350 administradores não licenciados. Os administradores licenciados continuarão a funcionar como estão, já que as associações transitivas se aplicam e não estão sujeitas ao limite de membro de 350.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 64dccfbfb99a4abdbd5232c899c736482cfbd119
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49226102"
---
# <a name="enableunlicensedadminstrators-action"></a>ação enableUnlicensedAdminstrators

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Após a habilitação, os usuários atribuídos como administradores por meio de associações de atribuição de função não precisarão mais de uma licença do Intune atribuída. Você está limitado a 350 membros diretos não licenciados para cada grupo de segurança do AAD em uma atribuição de função, mas você pode atribuir vários grupos de segurança do AAD a uma função se precisar dar suporte a mais de 350 administradores não licenciados. Os administradores licenciados continuarão a funcionar como estão, já que as associações transitivas se aplicam e não estão sujeitas ao limite de membro de 350.

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableUnlicensedAdminstrators
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
POST https://graph.microsoft.com/beta/deviceManagement/enableUnlicensedAdminstrators
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 204 No Content
```




