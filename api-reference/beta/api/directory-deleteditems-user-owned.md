---
title: Permissions
description: 'Recupera uma lista de itens excluídos recentemente pertencentes ao usuário especificado.  '
ms.openlocfilehash: 6d455fc7646c7e9c2b3fb62f48e098a5daeacff2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038124"
---
# <a name="list-deleted-items-owned-by-a-user"></a>**Listar itens excluídos pertencentes a um usuário**

Recupera uma lista de itens excluídos recentemente pertencentes ao usuário especificado.  

Atualmente, a funcionalidade de itens de lista excluída é suportada somente para [Agrupar](../resources/group.md) recursos pertencentes ao usuário.

Esta é uma ação de serviço, o que significa que ele não dá suporte a paginação.  A API retorna até 1.000 objetos excluídos pertencentes ao usuário, classificado por ID.  O usuário deve pertencer 1.000 ou mais excluído objetos, a API retorna nothing.

## <a name="permissions"></a>Permissions

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

| **Nome**      | **Descrição**           |
| ------------- | ------------------------- |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

```json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

O corpo da solicitação requer os seguintes parâmetros:

| Parâmetro    | Tipo |Descrição|
|:---------------|:--------|:----------|
|userId|String|ID do proprietário.|
|type|String|Tipo de objetos pertencentes para retornar; `Group` atualmente é o único valor com suporte.|

## <a name="response"></a>Resposta

Solicitações bem-sucedidas retornam `200 OK` códigos de resposta; o objeto de resposta inclui propriedades do [diretório (itens excluídos)](../resources/directory.md) .

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

``` http
POST https://graph.microsoft.com/beta/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"Group"
}
```

###### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. Observação: Este objeto de resposta pode estar truncado para fins de concisão. Todas as propriedades com suporte são retornadas de chamadas reais.

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": "2018-04-01T12:34:56Z",
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


