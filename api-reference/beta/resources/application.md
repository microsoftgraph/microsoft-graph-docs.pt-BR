---
title: tipo de recurso de aplicativo
description: 'Representa um aplicativo. Qualquer aplicativo que outsources autenticação do Azure Active Directory (AD Azure) deve ser registrado em um diretório. Registro de aplicativo envolve informando Azure AD sobre seu aplicativo, incluindo a URL onde ele tem localizado, a URL para enviar respostas após a autenticação, o URI para identificar o seu aplicativo e muito mais. Para obter mais informações, consulte Noções básicas sobre o registro de um aplicativo no Azure AD. Herda de directoryObject. '
localization_priority: Priority
ms.openlocfilehash: b64de5670ccb9deebbabe32bb691d15b5a621f30
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805667"
---
# <a name="application-resource-type"></a>tipo de recurso de aplicativo

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um aplicativo. Qualquer aplicativo que outsources autenticação do Azure Active Directory (AD Azure) deve ser registrado em um diretório. Registro de aplicativo envolve informando Azure AD sobre seu aplicativo, incluindo a URL onde ele tem localizado, a URL para enviar respostas após a autenticação, o URI para identificar o seu aplicativo e muito mais. Para obter mais informações, consulte [Noções básicas sobre o registro de um aplicativo no Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-authentication-scenarios/#basics-of-registering-an-application-in-azure-ad). Herda de [directoryObject](directoryobject.md). 

> **Observação:** Alterações para o tipo de recurso do aplicativo estejam atualmente em desenvolvimento. Para obter mais informações, consulte [problemas conhecidos com o Microsoft Graph](/graph/known-issues#application-and-serviceprincipal-api-changes).

Esse recurso permite:

- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/application-delta.md).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Obtenha o aplicativo](../api/application-get.md) | aplicativo |Leia as propriedades e os relacionamentos do objeto application.|
|[Criar aplicativo](../api/application-post-applications.md) | aplicativo | (Registradores) de cria um novo aplicativo.|
|[Lista de aplicativos](../api/application-list.md) | aplicativo | Recupere a lista de aplicativos na organização. |
|[Atualizar o aplicativo](../api/application-update.md) | aplicativo |Atualize o objeto application. |
|[Excluir aplicativo](../api/application-delete.md) | Nenhum |Exclua o objeto application. |
|[Políticas de lista atribuída](../api/policy-list-assigned.md)| coleção de [políticas](policy.md)| Obtenha todas as diretivas atribuídas a este objeto.|
|[Criar proprietário](../api/application-post-owners.md) |[directoryObject](directoryobject.md)| Crie um novo proprietário pelo lançamento à coleção proprietários.|
|[Listar proprietários](../api/application-list-owners.md) |Coleção [directoryObject](directoryobject.md)| Obtenha um proprietário de conjunto de objeto.|
|[delta](../api/application-delta.md)|conjunto de aplicativos| Obtenha as alterações incrementais para aplicativos. |
|[Criar chamada](../api/application-post-calls.md)|[chamada](call.md)|Crie uma nova chamada pelo lançamento à coleção de chamadas.|
|[Criar a reunião online](../api/application-post-onlinemeetings.md)|[onlineMeeting](onlinemeeting.md)|Crie uma nova reunião online, lançamento à coleção onlineMeetings.|

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|API|[API](api.md)| Especifica as configurações para um aplicativo de API. |
|appId| Cadeia de caracteres | O identificador exclusivo para o aplicativo que está atribuído a um aplicativo ao Azure AD. Não anulável. Somente leitura. |
|appRoles|coleção [appRole](approle.md)|A coleção de funções de aplicativos que um aplicativo pode declarar. Essas funções podem ser atribuídas a usuários, grupos ou entidades de serviço. Não anulável.|
|createdDateTime|DateTimeOffset| A data e hora que o aplicativo foi registrado. |
|deletedDateTime|DateTimeOffset| A data e hora que o aplicativo foi excluído. |
|displayName|Cadeia de caracteres|O nome de exibição para o aplicativo. |
|id|Cadeia de caracteres|O identificador exclusivo para o aplicativo. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura. |
|identifierUris|String collection| Os URIs que identifique o aplicativo. Para mais informações, consulte [objetos de aplicativo e objetos de entidade de serviço](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/). Operador *any* é necessário para expressões de filtro propriedades de valores múltiplos. Não anulável. |
|Info|[informationalUrl](informationalurl.md)| Informações básicas de perfil do aplicativo. |
|isFallbackPublicClient|Booliano| Especifica o tipo de aplicativo de fallback como cliente pública, como um aplicativo instalado em execução em um dispositivo móvel. O valor padrão é *false* indicando o tipo de aplicativo de fallback é confidencial cliente como o aplicativo web. Há determinadas situações em que o Azure AD não pode determinar o tipo de aplicativo cliente (por exemplo, fluxo [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3) onde ele está configurado sem a especificação de um URI de redirecionamento). Nesses casos Azure AD irá interpretar o tipo de aplicativo com base no valor dessa propriedade.|
|keyCredentials|coleção [keyCredential](keycredential.md)|O conjunto de credenciais principais associados ao aplicativo não anuláveis. |
|logotipo|Stream|O logotipo principal para o aplicativo. Não anulável. |
|optionalClaims|optionalClaims| Reservado para uso futuro. |
|orgRestrictions|String collection| Reservado para uso futuro. |
|parentalControlSettings|[parentalControlSettings](parentalcontrolsettings.md) |Especifica as configurações de controle do responsável para um aplicativo.|
|passwordCredentials|coleção [passwordCredential](passwordcredential.md)|A coleção de credenciais de senha associados ao aplicativo. Não anulável.|
|publicClient|[publicClient](publicclient.md)| Especifica as configurações para clientes instalados como os dispositivos móveis ou da área de trabalho. |
|publisherDomain| Cadeia de caracteres | O domínio verificado publisher para o aplicativo. Somente leitura.|
|requiredResourceAccess|coleção [requiredResourceAccess](requiredresourceaccess.md)|Especifica os recursos que esse aplicativo requer acesso aos e o conjunto de escopos de permissão do OAuth e funções de aplicativos que ele precisa em cada um desses recursos. Essa configuração prévia do acesso a recursos necessários drives a experiência de consentimento. Não anulável.|
|signInAudience | Cadeia de caracteres | Especifica quais contas da Microsoft são suportadas para o aplicativo atual. Valores suportados são:<ul><li>**AzureADMyOrg**: os usuários com o Microsoft trabalhar ou escola conta no locatário do Azure AD da minha organização (isto é, inquilino único)</li><li>**AzureADMultipleOrgs**: os usuários com o Microsoft trabalhar ou escola conta no locatário do Azure AD da organização, qualquer (ou seja, multilocatário)</li> <li>**AzureADandPersonalMicrosoftAccount**: os usuários com uma conta pessoal da Microsoft ou uma conta de trabalho ou da escola no locatário do Azure AD da organização, qualquer</li></ul> | `AzureADandPersonalMicrosoftAccount` |
|marcas|String collection| Cadeias de caracteres personalizadas que podem ser usadas para categorizar e identificar o aplicativo. |
|web|[Web](web.md)| Especifica as configurações para um aplicativo web. |

## <a name="relationships"></a>Relações

| Relação | Tipo | Descrição |
|:---------------|:--------|:----------|
|chamadas           |coleção de [chamada](call.md)                  |Somente leitura. Anulável.|
|connectorGroup|[connectorGroup](connectorgroup.md)| O connectorGroup o aplicativo está usando com Proxy de aplicativo do Windows Azure AD. Anulável.|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| Somente leitura.|
|onlineMeetings  |coleção [onlineMeeting](onlinemeeting.md)|Somente leitura. Anulável.|
|owners|Coleção [directoryObject](directoryobject.md)|Objetos de diretório que são proprietários do aplicativo. Os proprietários são um conjunto de usuários não seja o administrador que têm permissão para modificar esse objeto. Requer a versão 2013-11-08 ou mais recente. Somente leitura. Anulável.|
|Política|coleção de [políticas](policy.md)|As políticas atribuídas a esse aplicativo.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "createdOnBehalfOf",
    "owners"
  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "api": {"@odata.type": "microsoft.graph.apiApplication"},
  "appId": "String",
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}],
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "identifierUris": ["String"],
  "info": {"@odata.type": "microsoft.graph.informationalUrl"},
  "isFallbackPublicClient": true,
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logo": "Stream",
  "optionalClaims": [{"@odata.type": "microsoft.graph.optionalClaims"}],
  "orgRestrictions": ["Guid"],
  "parentalControlSettings": [{"@odata.type": "microsoft.graph.parentalControlSettings"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "preAuthorizedApplications": [{"@odata.type": "microsoft.graph.preAuthorizedApplication"}],
  "publicClient": {"@odata.type": "microsoft.graph.publicClientApplication"},
  "publisherDomain": "String",
  "requiredResourceAccess": [{"@odata.type": "microsoft.graph.requiredResourceAccess"}],
  "signInAudience": "String",
  "tags": ["String"],
  "web": {"@odata.type": "microsoft.graph.webApplication"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
