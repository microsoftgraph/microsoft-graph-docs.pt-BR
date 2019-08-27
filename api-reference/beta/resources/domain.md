---
title: tipo de recurso de domínio
description: Representa um domínio associado ao locatário.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dda30901f93661bafa8fe1a6d73f95a0cfdc4fb9
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633689"
---
# <a name="domain-resource-type"></a>tipo de recurso de domínio

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um domínio associado ao locatário.

Use as operações de domínio para associar domínios a um locatário, verificar a propriedade do domínio e configurar os serviços com suporte.  As operações de domínio habilitam registradores para automatizar a associação de domínios para serviços como o Office 365. Por exemplo, como parte do domínio inscrever-se, um registrador pode habilitar um domínio do personalizado para emails, sites, autenticação, etc.

Para associar um domínio a um locatário:

1. [Associar](../api/domain-post-domains.md) um domínio a um locatário.

2. [Recupere](../api/domain-list-verificationdnsrecords.md) os registros de verificação de domínio. Adicione os detalhes do registro de verificação ao arquivo de zona do domínio usando o registrador de domínio ou a configuração do servidor DNS.

3. [Verifique](../api/domain-verify.md) a propriedade do domínio. Isso verificará o domínio e definirá ** a propriedade isconfirmoud como *true*.

4. [Indicar](../api/domain-update.md) os serviços com suporte que você planeja usar com o domínio.

5. [Configure](../api/domain-list-serviceconfigurationrecords.md) os serviços com suporte ao recuperar uma lista de registros necessários para habilitar os serviços do domínio. Adicione os detalhes do registro de configuração ao arquivo de zona do domínio usando o registrador de domínio ou a configuração do servidor DNS.

## <a name="methods"></a>Métodos

| Método   | Tipo de retorno |Descrição|
|:---------------|:--------|:----------|
|[Obter domínio](../api/domain-get.md) | [domain](domain.md) | Leia as propriedades e as relações de um objeto de domínio.|
|[Criar domínio](../api/domain-post-domains.md) | [domain](domain.md) | Adiciona um domínio ao inquilino. |
|[Listar domainNameReference](../api/domain-list-domainnamereferences.md) |Coleção [directoryObject](directoryobject.md)| Recupere uma lista de objetos de diretório com uma referência ao domínio.|
|[Listar serviceConfigurationRecords](../api/domain-list-serviceconfigurationrecords.md) |coleção [domainDnsRecord](domaindnsrecord.md)|  Recupere uma lista de registros DNS de domínio para configuração de domínio.|
|[Listar verificationDnsRecords](../api/domain-list-verificationdnsrecords.md) |coleção [domainDnsRecord](domaindnsrecord.md)|  Recupere uma lista de registros DNS de domínio para verificação de domínio.|
|[Atualizar domínio](../api/domain-update.md) | [domain](domain.md) |Atualiza um domínio.|
|[Excluir domínio](../api/domain-delete.md) | Nenhum |Exclui um domínio.|
|[Domínio ForceDelete](../api/domain-forcedelete.md)|Nenhum|Exclui um domínio usando uma operação assíncrona.|
|[Verificar domínio](../api/domain-verify.md)|[domain](domain.md)|Valida a propriedade do domínio.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo | Descrição |
|:---------------|:--------|:----------|
|authenticationType|String| Indica o tipo de autenticação configurada para o domínio. O valor é *gerenciado* ou *federado*.<br> *Gerenciado* indica um domínio gerenciado em nuvem onde o Azure ad realiza autenticação do usuário.<br>*Federado* indica que a autenticação é federada com um provedor de identidade, como o Active Directory local do locatário por meio dos serviços de Federação do Active Directory. Isso é somente leitura e não é anulável. |
|availabilityStatus|String| Essa propriedade é sempre NULL, exceto quando a ação [Verify](../api/domain-verify.md) é usada. Quando a ação [Verify](../api/domain-verify.md) é usada, uma entidade de **domínio** é retornada na resposta. A propriedade **availabilityStatus** da entidade de **domínio** na resposta é *AvailableImmediately* ou *EmailVerifiedDomainTakeoverScheduled*.|
|id|String| O nome totalmente qualificado do domínio. Key, imutável, não anulável, exclusivo |
|isAdminManaged|Booliano| O valor da propriedade será false se o gerenciamento de registro DNS do domínio tiver sido delegado para o Office 365. Caso contrário, o valor será true. Não anulável |
|isDefault|Booliano| True se este é o domínio padrão usado para a criação de usuários. Há apenas um domínio padrão por empresa. Não anulável |
|isinitial|Booliano| True se este é o domínio inicial criado pelo Microsoft Online Services (companyname.onmicrosoft.com). Há apenas um domínio inicial por empresa. Não anulável |
|IsRoot|Booliano| True se o domínio é um domínio raiz verificado. Caso contrário, false se o domínio é um subdomínio ou não verificado. Não anulável |
|isverificed|Booliano| True se o domínio tiver concluído a verificação de propriedade de domínio. Não anulável |
|passwordNotificationWindowInDays|Int32|Especifica o número de dias antes que um usuário receba uma notificação de que a senha expirará. Se a propriedade não for definida, será usado um valor padrão de 14 dias.|
|passwordValidityPeriodInDays|Int32| Especifica o período de tempo que uma senha é válida antes de ser alterada. Se a propriedade não for definida, será usado um valor padrão de 90 dias. |
|supportedservices|Coleção de cadeias de caracteres| Os recursos atribuídos ao domínio.<br><br>Pode incluir 0, 1 ou mais dos seguintes valores: *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*<br><br> Os valores que você pode adicionar/remover usando a API do Graph incluem: *email*, *OfficeCommunicationsOnline*, *Yammer*<br>Não anulável|
|estado|[domainstate](domainstate.md)| Status das operações assíncronas agendadas para o domínio. |

## <a name="relationships"></a>Relações

As relações entre um domínio e outros objetos no diretório, como seus registros de verificação e registros de configuração de serviço, são expostas por meio das propriedades de navegação. Você pode ler essas relações direcionando essas propriedades de navegação em suas solicitações.

| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|domainNameReferences|Coleção [directoryObject](directoryobject.md)| Somente leitura, anulável|
|serviceConfigurationRecords|coleção [domainDnsRecord](domaindnsrecord.md)| Os registros DNS que o cliente adiciona ao arquivo de zona DNS do domínio antes que o domínio possa ser usado pelo Microsoft Online Services.<br>Somente leitura, anulável |
|verificationDnsRecords|coleção [domainDnsRecord](domaindnsrecord.md)| Registros DNS que o cliente adiciona ao arquivo de zona DNS do domínio antes que o cliente possa concluir a verificação de propriedade de domínio com o Azure AD.<br>Somente leitura, anulável|

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
