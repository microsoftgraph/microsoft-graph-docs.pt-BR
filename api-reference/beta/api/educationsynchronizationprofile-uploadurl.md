---
title: 'educationSynchronizationProfile: uploadUrl'
description: Recupere uma assinatura de acesso compartilhado (SAS) para o carregamento de arquivos de origem para o armazenamento de blob Azure para um perfil de sincronização de dados específicos escola no inquilino. O token SAS tem uma validade de uma hora.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e0119a583ea1cdc753b44a984af84a42173a4295
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969909"
---
# <a name="educationsynchronizationprofile-uploadurl"></a>educationSynchronizationProfile: uploadUrl

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Recupere uma assinatura de acesso compartilhado (SAS) para carregar arquivos de origem para o armazenamento de blob Azure para um de dados específicos escola [perfil de sincronização](../resources/educationsynchronizationprofile.md) no inquilino. O token SAS tem uma validade de uma hora.

O carregamento URL é fornecido apenas para o [provedor de dados CSV](../resources/educationcsvdataprovider.md).

> **Observação:** Para acessar o armazenamento de blob com o token SAS, use o [armazenamento do Azure SDKs](https://github.com/search?q=org%3AAzure+azure-storage) ou [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões |
|:-----------|:----------|
| Delegado (conta corporativa ou de estudante) | EduAdministration.ReadWrite |
|Delegada (conta pessoal da Microsoft|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.
## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e uma URL de SAS para o [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) no corpo da resposta.

Se uma solicitação anterior ainda está sendo processada, esse método retorna um `409 Conflict` indicando que o carregamento momento seja bloqueado para o [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```

##### <a name="response"></a>Resposta
Este é um exemplo de resposta. 

>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "@odata.type": "String",
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 314

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#String",
    "value": "https://sdsstorage.blob.core.windows.net/86904b1e-c7d0-4ead-b13a-98f11fc400ee?sv=2015-07-08&sr=c&si=SharedAccessPolicy_20170704044441&sig=CH65vxxqXETCkQNH0Lfsu31cUo0s0XcEEo0OE2YiL6Q%3D&se=2017-07-04T08%3A43%3A01Z&sp=w"
}
```
