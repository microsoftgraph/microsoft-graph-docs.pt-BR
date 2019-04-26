---
title: Atualizar aplicativo
description: Atualiza as propriedades do objeto Application.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3c85608ad31d0d83607a49e06e2a46032e927bc4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322891"
---
# <a name="update-application"></a>Atualizar aplicativo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualiza as propriedades do objeto Application.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Application.ReadWrite.OwnedBy, Application.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Allowpublicclient e|Boolean| Especifica se o aplicativo pode atuar como um cliente público. Por exemplo, um aplicativo instalado em execução em um dispositivo móvel. O valor padrão é *false*. |
|api|[apiApplication](../resources/apiapplication.md)| Especifica configurações para um aplicativo de API. |
|appRoles|Coleção [appRole](../resources/approle.md)|A coleção de funções de aplicativo que um aplicativo pode declarar. Essas funções podem ser atribuídas a usuários, grupos ou entidades de serviço. Não anulável.|
|É applicationaliases|Coleção String| Os URIs que identificam o aplicativo. Para saber mais, confira [Objetos do aplicativo e objetos da entidade de serviço](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/). O operador *any* é obrigatório para expressões de filtro em propriedades de vários valores. Não anulável. |
|createdDateTime|DateTimeOffset| A data e a hora que o aplicativo foi registrado. |
|deletedDateTime|DateTimeOffset| A data e a hora que o aplicativo foi excluído. |
|displayName|String|O nome de exibição do aplicativo. |
|id|String|O identificador exclusivo do aplicativo. Herdado de [directoryObject](../resources/directoryobject.md). Chave. Não anulável. Somente leitura. |
|informações |[informationalUrl](../resources/informationalurl.md)| Informações de perfil básicas do aplicativo. | Especifica configurações para clientes instalados, como dispositivos móveis ou da área de trabalho. |
|keyCredentials|Coleção [keyCredential](../resources/keycredential.md)|A coleção de credenciais chaves associada ao aplicativo Não anulável. |
|logo|Stream|O principal logotipo do aplicativo. Não anulável. |
|orgRestrictions|Coleção String| A organização tenantIds à qual o aplicativo é restrito.  Se a coleção estiver vazia, o aplicativo será multilocatário (não restrito). Se a coleção contiver tenantIds, o aplicativo será restrito ao tenantIds organizacional na coleção. A especificação de outros locatários, mas não o tenantid onde o aplicativo está registrado indica que a própria tenantid do aplicativo está indiretamente incluída. |
|passwordCredentials|Coleção [passwordCredential](../resources/passwordcredential.md)|A coleção de credenciais de senha associada ao aplicativo. Não anulável.|
|preAuthorizedApplications|coleção [preauthorizedapplication e](../resources/preauthorizedapplication.md)| Lista os aplicativos e as permissões solicitadas para o consentimento implícito. Requer um administrador para ter fornecido o consentimento para o aplicativo. o preAuthorizedApplications não exige que o usuário concorde com as permissões solicitadas. As permissões listadas no preAuthorizedApplications não exigem o consentimento do usuário. No enTanto, as permissões adicionais solicitadas não listadas no preAuthorizedApplications exigem o consentimento do usuário. |
|requiredResourceAccess|[requiredResourceAccess](../resources/requiredresourceaccess.md) collection|Especifica os recursos para os quais esse aplicativo requer acesso e o conjunto de escopos de permissão e funções de aplicativo do OAuth necessários em cada um desses recursos. Essa pré-configuração de acesso necessário aos recursos impulsiona a experiência de consentimento. Não anulável.|
|tags|Coleção String| Sequências personalizadas que podem ser usadas para categorizar e identificar o aplicativo. |
|web|[webApplication](../resources/webApplication.md)| Especifica configurações para um aplicativo Web. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `204 No Content` um código de resposta e não retornará nada no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->
```http
PATCH https://graph.microsoft.com/beta/applications/{id}
Content-type: application/json
Content-length: 72

{
  "allowPublicClient": false,
  "displayName": "New display name"
}
```
##### <a name="response"></a>Resposta
Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
