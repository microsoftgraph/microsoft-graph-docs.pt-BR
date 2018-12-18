---
title: Atualizar o aplicativo
description: Atualize as propriedades do objeto application.
author: lleonard-msft
ms.openlocfilehash: e664e212f81bab9f4e8b49bce60b4ec045fa5787
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316685"
---
# <a name="update-application"></a>Atualizar o aplicativo

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Atualize as propriedades do objeto application.
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
|allowPublicClient|Boolean| Especifica se o aplicativo pode atuar como um cliente público. Por exemplo, um aplicativo instalado em execução em um dispositivo móvel. O valor padrão é *false*. |
|API|[API](../resources/api.md)| Especifica as configurações para um aplicativo de API. |
|appRoles|coleção [appRole](../resources/approle.md)|A coleção de funções de aplicativos que um aplicativo pode declarar. Essas funções podem ser atribuídas a usuários, grupos ou entidades de serviço. Não anulável.|
|applicationAliases|String collection| Os URIs que identifique o aplicativo. Para mais informações, consulte [objetos de aplicativo e objetos de entidade de serviço](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/). Operador *any* é necessário para expressões de filtro propriedades de valores múltiplos. Não anulável. |
|createdDateTime|DateTimeOffset| A data e hora que o aplicativo foi registrado. |
|deletedDateTime|DateTimeOffset| A data e hora que o aplicativo foi excluído. |
|displayName|String|O nome de exibição para o aplicativo. |
|id|String|O identificador exclusivo para o aplicativo. Herdado de [directoryObject](../resources/directoryobject.md). Chave. Não anulável. Somente leitura. |
|Info|[informationalUrl](../resources/informationalurl.md)| Informações básicas de perfil do aplicativo. | Especifica as configurações para clientes instalados como os dispositivos móveis ou da área de trabalho. |
|keyCredentials|coleção [keyCredential](../resources/keycredential.md)|O conjunto de credenciais principais associados ao aplicativo não anuláveis. |
|logotipo|Stream|O logotipo principal para o aplicativo. Não anulável. |
|orgRestrictions|String collection| O tenantIds organizacional à qual o aplicativo é restrito.  Se a coleção estiver vazia, o aplicativo está multilocatário (não restrito). Se a coleção contiver tenantIds, o aplicativo é restrito ao tenantIds organizacional na coleção. Especificar outros tenants, mas não a tenantId em que o aplicativo está registrado implica que a tenantId do aplicativo é indiretamente incluída. |
|passwordCredentials|coleção [passwordCredential](../resources/passwordcredential.md)|A coleção de credenciais de senha associados ao aplicativo. Não anulável.|
|preAuthorizedApplications|coleção [preAuthorizedApplication](../resources/preauthorizedapplication.md)| Lista de aplicativos e as permissões solicitadas para consentimento implícito. Requer um administrador tenha fornecido a consentimento para o aplicativo. preAuthorizedApplications não exigem o usuário concorda com as permissões solicitadas. Permissões listadas na preAuthorizedApplications não exigem consentimento do usuário. No entanto, qualquer permissões solicitadas adicionais não listados no preAuthorizedApplications exigem o consentimento do usuário. |
|requiredResourceAccess|coleção [requiredResourceAccess](../resources/requiredresourceaccess.md)|Especifica os recursos que esse aplicativo requer acesso aos e o conjunto de escopos de permissão do OAuth e funções de aplicativos que ele precisa em cada um desses recursos. Essa configuração prévia do acesso a recursos necessários drives a experiência de consentimento. Não anulável.|
|marcas|String collection| Cadeias de caracteres personalizadas que podem ser usadas para categorizar e identificar o aplicativo. |
|web|[Web](../resources/web.md)| Especifica as configurações para um aplicativo web. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `204 No Content` código de resposta e não retornará nada no corpo da resposta.
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
<!-- {
  "type": "#page.annotation",
  "description": "Update application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->