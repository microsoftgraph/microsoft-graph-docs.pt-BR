---
title: Ação enableUnlicensedAdminstrators
description: Após a habilitação, os usuários atribuídos como administradores por meio de Associações de Atribuição de Função não exigirão mais uma licença atribuída do Intune. Você está limitado a 350 membros diretos sem licença para cada grupo de segurança do AAD em uma atribuição de função, mas pode atribuir vários grupos de segurança do AAD a uma função se precisar dar suporte a mais de 350 administradores não licenças. Os administradores licenciados continuarão a funcionar como estão na medida em que as associações transitivas se aplicam e não estão sujeitas ao limite de 350 membros.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1b62a4316f1faf04812571fdffed94d6b14ca12f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59061167"
---
# <a name="enableunlicensedadminstrators-action"></a>Ação enableUnlicensedAdminstrators

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Após a habilitação, os usuários atribuídos como administradores por meio de Associações de Atribuição de Função não exigirão mais uma licença atribuída do Intune. Você está limitado a 350 membros diretos sem licença para cada grupo de segurança do AAD em uma atribuição de função, mas pode atribuir vários grupos de segurança do AAD a uma função se precisar dar suporte a mais de 350 administradores não licenças. Os administradores licenciados continuarão a funcionar como estão na medida em que as associações transitivas se aplicam e não estão sujeitas ao limite de 350 membros.

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All|

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



