---
title: Listar privilegedOperationEvents
description: Recupere eventos de auditoria gerados pelo PIM para operações de função.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: 5eaafd77c903a006bdfb01a077de1a006b34ac9d
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694712"
---
# <a name="list-privilegedoperationevents"></a>Listar privilegedOperationEvents

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v1AADRoles-deprecation](../../includes/pim-v1aadroles-deprecation.md)]

Recupere uma lista de objetos [privilegedOperationEvent,](../resources/privilegedoperationevent.md) que representam os eventos de auditoria gerados pelo Privileged Identity Management para as operações de função. Para obter os detalhes sobre o evento de auditoria, consulte [privilegedOperationEvent](../resources/privilegedoperationevent.md). Para filtrar os resultados da consulta, use a expressão OData ``$filter`` padrão.


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

O solicitante precisa ter uma das seguintes funções: Administrador de Função _Privilegiada,_ _Administrador Global,_ Administrador de Segurança _ou_ Leitor de _Segurança._

 

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedOperationEvents
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [privilegedOperationEvent](../resources/privilegedoperationevent.md) no corpo da resposta.

Observe que o locatário precisa ser registrado no PIM. Caso contrário, o código de status HTTP 403 Forbidden será retornado.
## <a name="examples"></a>Exemplos

### <a name="get-audit-events-for-role-assignment-operations"></a>Obter eventos de auditoria para operações de atribuição de função
##### <a name="request"></a>Solicitação
O exemplo a seguir mostra uma solicitação para obter os eventos de auditoria para as operações de atribuição de função. Nesse caso, o ``requestType`` valor é ``Assign`` .

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/beta/privilegedOperationEvents?$filter=requestType%20eq%20'Assign'
```
##### <a name="response"></a>Resposta
O exemplo a seguir mostra a resposta. Observação: O objeto de resposta exibido aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedOperationEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 547

{
    "value": [
        {
            "id": "201707240003469369",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f80",
            "userName": "admin1",
            "userMail": "admin1@contoso.onmicrosoft.com",
            "roleId": "9360feb5-f418-4baa-8175-e2a00bac4301",
            "roleName": "Directory Writers",
            "expirationDateTime": "0001-01-01T00:00:00Z",
            "creationDateTime": "2017-07-24T18:32:38.7589078Z",
            "requestorId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "requestorName": "admin",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Assign",
            "additionalInformation": null,
            "referenceKey": null,
            "referenceSystem": null
        },
        {
            "id": "201707240003469372",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f80",
            "userName": "admin",
            "userMail": "admin1@contoso.onmicrosoft.com",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "roleName": "Guest Inviter",
            "expirationDateTime": "0001-01-01T00:00:00Z",
            "creationDateTime": "2017-07-24T18:33:00.7607701Z",
            "requestorId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "requestorName": "admin",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Assign",
            "additionalInformation": null,
            "referenceKey": null,
            "referenceSystem": null
        }
    ]
}
```
### <a name="get-audit-events-for-the-operations-of-self-role-activation-and-makepermanent"></a>Obter eventos de auditoria para as operações de ativação de auto-função e makePermanent
##### <a name="request"></a>Solicitação
O exemplo a seguir mostra uma solicitação para obter os eventos de auditoria para as operações de ativação de auto-função e makePermanent. Nesse caso, o ``requestType`` valor é ``Activate`` .

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/beta/privilegedOperationEvents?$filter=requestType%20eq%20'Activate'
```
##### <a name="response"></a>Resposta
O exemplo a seguir mostra a resposta. Observação: O objeto de resposta exibido aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedOperationEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 547

{
    "value": [
        {
            "id": "201707240003469811",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "userName": "admin1",
            "userMail": "admin1@contoso.onmicrosoft.com",
            "roleId": "44367163-eba1-44c3-98af-f5787879f96a",
            "roleName": "CRM Service Administrator",
            "expirationDateTime": "0001-01-01T00:00:00Z",
            "creationDateTime": "2017-07-24T23:34:41.9661094Z",
            "requestorId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "requestorName": "admin1",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Activate",
            "additionalInformation": "Make permanent admin",
            "referenceKey": null,
            "referenceSystem": null
        },
        {
            "id": "201707240003469814",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "userName": "admin1",
            "userMail": "admin1@contoso.onmicrosoft.com",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "roleName": "Guest Inviter",
            "expirationDateTime": "2017-07-25T00:37:07.3402169Z",
            "creationDateTime": "2017-07-24T23:37:08.0052112Z",
            "requestorId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "requestorName": "admin1",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Activate",
            "additionalInformation": "self activate",
            "referenceKey": "",
            "referenceSystem": ""
        }
    ]
}
```

### <a name="get-audit-events-for-role-assignment-deactivation"></a>Obter eventos de auditoria para desativação de atribuição de função
##### <a name="request"></a>Solicitação
O exemplo a seguir mostra uma solicitação para obter os eventos de auditoria para desativação da atribuição de função. Nesse caso, o ``requestType`` valor é ``Deactivate`` .

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/beta/privilegedOperationEvents?$filter=requestType%20eq%20'Deactivate'
```
##### <a name="response"></a>Resposta
O exemplo a seguir mostra a resposta. Observação: O objeto de resposta exibido aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedOperationEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 547

{
    "value": [
        {
            "id": "201707240003469375",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f80",
            "userName": "admin1",
            "userMail": "admin1@contoso.onmicrosoft.com",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "roleName": "Guest Inviter",
            "expirationDateTime": "0001-01-01T00:00:00Z",
            "creationDateTime": "2017-07-24T18:33:28.3408971Z",
            "requestorId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "requestorName": "admin1",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Deactivate",
            "additionalInformation": "Make eligible admin",
            "referenceKey": null,
            "referenceSystem": null
        }
    ]
}
```
### <a name="get-audit-events-created-in-a-time-range"></a>Obter eventos de auditoria criados em um intervalo de tempo
##### <a name="request"></a>Solicitação 
O exemplo a seguir mostra uma solicitação para obter os eventos de auditoria criados em um intervalo de tempo.

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/beta/privilegedOperationEvents?$filter=(creationDateTime%20ge%202017-06-25T07:00:00Z)%20and%20(creationDateTime%20le%202017-07-25T17:30:17Z)&$count=true&$orderby=creationDateTime%20desc
```
##### <a name="response"></a>Resposta
O exemplo a seguir mostra a resposta. Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedOperationEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 547

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedOperationEvents",
    "@odata.count": 2,
    "value": [
        {
            "id": "201707250003471056",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "userName": "admin",
            "userMail": "admin@contoso.onmicrosoft.com",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "roleName": "Guest Inviter",
            "expirationDateTime": "2017-07-25T17:38:49.5640383Z",
            "creationDateTime": "2017-07-25T16:38:50.3681771Z",
            "requestorId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "requestorName": "admin",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Activate",
            "additionalInformation": "activate test",
            "referenceKey": "",
            "referenceSystem": ""
        },
        {
            "id": "201707250003469896",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "userName": "admin",
            "userMail": "admin@contoso.onmicrosoft.com",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "roleName": "Guest Inviter",
            "expirationDateTime": "0001-01-01T00:00:00Z",
            "creationDateTime": "2017-07-25T00:37:08.6172407Z",
            "requestorId": "6b61baec-bb80-4a8a-b8bd-fa5ba1f12386",
            "requestorName": "Azure AD PIM",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Deactivate",
            "additionalInformation": "Expired",
            "referenceKey": "",
            "referenceSystem": ""
        }
    ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedOperationEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
