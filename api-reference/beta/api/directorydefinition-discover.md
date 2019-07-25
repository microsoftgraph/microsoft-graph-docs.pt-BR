---
title: 'directoryDefinition: descobrir'
description: 'Descubra a definição de esquema mais recente para provisionamento para um aplicativo. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aafd4ad57d8e6d75ebdcd3c7bf2fba4506e48f56
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879574"
---
# <a name="directorydefinition-discover"></a>directoryDefinition: descobrir

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descubra a definição de esquema mais recente para provisionamento para um aplicativo. 

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Directory.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Somente aplicativo                            | Nenhum. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor                      |
|:--------------|:---------------------------|
| Autorização | {token} do portador (obrigatório)  |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método. 

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` uma resposta com um objeto [directoryDefinition](../resources/synchronization-directorydefinition.md) .

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "discover_directorydefinition"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```

### <a name="response"></a>Resposta

Veja a seguir um exemplo de uma resposta.

>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "discoverabilities": "AttributeNames, AttributeDataTypes",
  "discoveryDateTime": "2019-03-20T15:47:50.4707552Z",
  "id": "directoryDefinitionId",
  "objects": [{
        "name": "User",
        "attributes": [{
                "name": "Id",
                "type": "String"
            }, {
                "name": "FirstName",
                "type": "String"
            },
            {
                "name": "CustomExendedAttribute",
                "type": "String"
            }  
        ]
    }],
  "version": "bf8c03ac-d45e-47fe-b3a1-711a9418b2b1"
}
 ```
