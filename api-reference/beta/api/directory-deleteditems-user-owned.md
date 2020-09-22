---
title: Listar itens excluídos pertencentes a um usuário
description: 'Recupera uma lista de itens excluídos recentemente pertencentes ao usuário especificado.  '
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 84d0c9d688ef67fa36354c4cc037ecb61777eb0d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008915"
---
# <a name="list-deleted-items-owned-by-a-user"></a>Listar itens excluídos pertencentes a um usuário

Namespace: microsoft.graph

Recupera uma lista de itens excluídos recentemente pertencentes ao usuário especificado.  

Atualmente, a funcionalidade Listar itens excluídos é suportada apenas para recursos de [aplicativo](../resources/application.md) e de [grupo](../resources/group.md) pertencentes ao usuário.

Esta é uma ação de serviço, o que significa que ele não oferece suporte à paginação.  A API retorna até 1.000 objetos excluídos pertencentes ao usuário, classificados por ID.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
| --- | --- |
| Delegado (conta corporativa ou de estudante) | Group.Read.All, Group.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) |  Sem suporte. |
| Aplicativo | Group.Read.All, Group.ReadWrite.All  |

## <a name="http-request"></a>Solicitação HTTP

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| ------------- | ------------------------- |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

O corpo da solicitação requer os seguintes parâmetros:

| Parâmetro    | Tipo |Descrição|
|:---------------|:--------|:----------|
|userId|Cadeia de caracteres|ID do proprietário.|
|tipo|String|Tipo de objetos de propriedade a ser retornado; `group` no momento, o único valor com suporte.|


## <a name="response"></a>Resposta

Solicitações bem-sucedidas retornam `200 OK` códigos de resposta; o objeto Response inclui as propriedades [Directory (Deleted Items)](../resources/directory.md) .

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

``` http
POST https://graph.microsoft.com/beta/directory/deletedItems/getUserOwnedObjects
Content-type: application/json

{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. Observação: esse objeto de resposta pode ser truncado por brevidade. Todas as propriedades com suporte são retornadas de chamadas reais.

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": "2018-04-01T12:39:16Z",
              "classification": null,
              "createdDateTime": "2017-03-22T12:39:16Z",
              "description": null,
              "displayName": "Test",
              "groupTypes": [
                  "Unified"
              ],
              "mail": "Test@contoso.com",
              "mailEnabled": true,
              "mailNickname": "Test",
              "membershipRule": null,
              "membershipRuleProcessingState": null,
              "preferredDataLocation": null,
              "preferredLanguage": null,
              "proxyAddresses": [
                  "SMTP:Test@contoso.com"
              ],
              "renewedDateTime": "2017-09-22T22:30:39Z",
              "securityEnabled": false,
              "theme": null,
              "visibility": "Public"
          } 
        ]
 }
```




