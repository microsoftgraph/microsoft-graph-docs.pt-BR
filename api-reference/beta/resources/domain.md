---
title: tipo de recurso de domínio
description: Representa um domínio associado ao locatário.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: d22df53e3d274601d58f17cbbf859de47ae3d1f9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440399"
---
# <a name="domain-resource-type"></a>tipo de recurso de domínio

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um domínio associado ao locatário.

Use operações de domínio para associar domínios a um locatário, verificar a propriedade do domínio e configurar serviços com suporte.  As operações de domínio permitem que os registradores automatizem a associação de domínio para serviços como o Microsoft 365. Por exemplo, como parte da inscrição no domínio, um registrador pode habilitar um domínio de vaidade para email, sites, autenticação etc.

Para associar um domínio a um locatário:

1. [Associe](../api/domain-post-domains.md) um domínio a um locatário.

2. [Recupere](../api/domain-list-verificationdnsrecords.md) os registros de verificação de domínio. Adicione os detalhes do registro de verificação ao arquivo de zona do domínio usando o registrador de domínio ou a configuração do servidor DNS.

3. [Verifique](../api/domain-verify.md) a propriedade do domínio. Isso verificará o domínio e definirá a *propriedade isVerified* como *true*.

4. [Indique](../api/domain-update.md) os serviços com suporte que você planeja usar com o domínio.

5. [Configure](../api/domain-list-serviceconfigurationrecords.md) os serviços com suporte recuperando uma lista de registros necessários para habilitar serviços para o domínio. Adicione os detalhes do registro de configuração ao arquivo de zona do domínio usando o registrador de domínio ou a configuração do servidor DNS.

## <a name="methods"></a>Methods

| Método   | Tipo de retorno |Descrição|
|:---------------|:--------|:----------|
|[Obter domínio](../api/domain-get.md) | [domain](domain.md) | Ler propriedades e relações de um objeto de domínio.|
|[Criar domínio](../api/domain-post-domains.md) | [domain](domain.md) | Adiciona um domínio ao inquilino. |
|[Listar domainNameReference](../api/domain-list-domainnamereferences.md) |Coleção [directoryObject](directoryobject.md)| Recupere uma lista de objetos de diretório com uma referência ao domínio.|
|[Listar serviceConfigurationRecords](../api/domain-list-serviceconfigurationrecords.md) |[coleção domainDnsRecord](domaindnsrecord.md)|  Recupere uma lista de registros DNS de domínio para configuração de domínio.|
|[Listar verificationDnsRecords](../api/domain-list-verificationdnsrecords.md) |[coleção domainDnsRecord](domaindnsrecord.md)|  Recupere uma lista de registros DNS de domínio para verificação de domínio.|
|[Atualizar domínio](../api/domain-update.md) | [domain](domain.md) |Atualiza um domínio.|
|[Excluir domínio](../api/domain-delete.md) | Nenhum(a) |Exclui um domínio.|
|[Domínio ForceDelete](../api/domain-forcedelete.md)|Nenhum(a)|Exclui um domínio usando uma operação assíncrona.|
|[Verificar domínio](../api/domain-verify.md)|[domain](domain.md)|Valida a propriedade do domínio.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo | Descrição |
|:---------------|:--------|:----------|
|authenticationType|String| Indica o tipo de autenticação configurado para o domínio. O valor é *Gerenciado* ou *Federado.*<br> *Gerenciado* indica um domínio gerenciado na nuvem em que o Azure AD executa a autenticação do usuário.<br>*Federado* indica que a autenticação é federada com um provedor de identidade, como o Active Directory local do locatário por meio dos Serviços de Federação do Active Directory. Esse propert é somente leitura e não é anulado. |
|availabilityStatus|String| Essa propriedade é sempre nula, exceto quando [a ação de verificação](../api/domain-verify.md) é usada. Quando a [ação verify](../api/domain-verify.md) é usada, uma entidade **de** domínio é retornada na resposta. A **propriedade availabilityStatus** da entidade **de** domínio na resposta é *AvailableImmediately* ou *EmailVerifiedDomainTakeoverScheduled*.|
|id|String| O nome totalmente qualificado do domínio. Chave, imutável, não anulada, exclusiva |
|isAdminManaged|Booliano| O valor da propriedade será false se o gerenciamento de registro DNS do domínio tiver sido delegado ao Microsoft 365. Caso contrário, o valor será verdadeiro. Não anulada |
|isDefault|Booliano| True se esse for o domínio padrão usado para a criação do usuário. Há apenas um domínio padrão por empresa. Não anulada |
|isInitial|Booliano| True se esse for o domínio inicial criado por Microsoft Online Services (companyname.onmicrosoft.com). Há apenas um domínio inicial por empresa. Não anulada |
|isRoot|Booliano| True se o domínio for um domínio raiz verificado. Caso contrário, false se o domínio for um subdomínio ou não verificado. Não anulada |
|isVerified|Booliano| True se o domínio concluiu a verificação de propriedade do domínio. Não anulada |
|passwordNotificationWindowInDays|Int32|Especifica o número de dias antes de um usuário receber uma notificação de que sua senha expirará. Se a propriedade não estiver definida, um valor padrão de 14 dias será usado.|
|passwordValidityPeriodInDays|Int32| Especifica o período de tempo em que uma senha é válida antes de ser alterada. Se a propriedade não estiver definida, um valor padrão de 90 dias será usado. |
|supportedServices|Coleção de cadeias de caracteres| Os recursos atribuídos ao domínio.<br><br>Pode incluir 0, 1 ou mais dos seguintes valores: *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*<br><br> Os valores que você pode adicionar/remover usando a API do Graph incluem: *Email*, *OfficeCommunicationsOnline*, *Yammer*<br>Não anulada|
|state|[domainState](domainstate.md)| Status de operações assíncronas agendadas para o domínio. |

## <a name="relationships"></a>Relações

As relações entre um domínio e outros objetos no diretório, como seus registros de verificação e registros de configuração de serviço, são expostas por meio de propriedades de navegação. Você pode ler essas relações direcionando essas propriedades de navegação em suas solicitações.

| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|domainNameReferences|Coleção [directoryObject](directoryobject.md)| Somente leitura, Nullable|
|serviceConfigurationRecords|[coleção domainDnsRecord](domaindnsrecord.md)| O DNS registra que o cliente adiciona ao arquivo de zona DNS do domínio antes que o domínio possa ser usado pelos serviços do Microsoft Online.<br>Somente leitura, Nullable |
|verificationDnsRecords|[coleção domainDnsRecord](domaindnsrecord.md)| Registros DNS que o cliente adiciona ao arquivo de zona DNS do domínio antes que o cliente possa concluir a verificação de propriedade de domínio com o Azure AD.<br>Somente leitura, Nullable|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domain"
}-->

```json
{
  "authenticationType": "String",
  "availabilityStatus": "String",
  "id": "String (identifier)",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "passwordNotificationWindowInDays": 14,
  "passwordValidityPeriodInDays": 90,
  "state": {"@odata.type": "microsoft.graph.domainState"},
  "supportedServices": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


