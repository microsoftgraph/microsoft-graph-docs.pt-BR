---
title: Listar managedEBookCategories
description: Listar propriedades e relações dos objetos managedEBookCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9591ecd5c167087da816501b5011ffa05a228958
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133000"
---
# <a name="list-managedebookcategories"></a>Listar managedEBookCategories

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Listar propriedades e relações dos [objetos managedEBookCategory.](../resources/intune-books-managedebookcategory.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBookCategories
GET /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos managedEBookCategory](../resources/intune-books-managedebookcategory.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 264

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBookCategory",
      "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




