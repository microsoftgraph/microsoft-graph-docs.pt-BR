---
title: tipo de recurso de domínio
description: Representa um domínio associado ao locatário.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5d8dabf29285aea0b24613e584184dc13e02e499
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942392"
---
# <a name="domain-resource-type"></a>tipo de recurso de domínio

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um domínio associado ao locatário.

Use operações de domínio para associá-los a um locatário, verificar a propriedade do domínio e configurar os serviços com suporte.  Operações de domínio permitem que os registradores automatizem a associação de domínio para os serviços como o Office 365. Por exemplo, como parte da inscrição no domínio, um registrador pode habilitar um domínio personalizado para emails, sites, autenticação etc.

Para associar um domínio a um locatário:

1. [Associar](../api/domain-post-domains.md) um domínio a um locatário.

2. [Recuperar](../api/domain-list-verificationdnsrecords.md) os registros de verificação do domínio. Adicione os detalhes de registro de verificação ao arquivo de zona do domínio usando o registrador de domínio ou a configuração do servidor DNS.

3. [Verifica](../api/domain-verify.md) a propriedade do domínio. Isso verificará o domínio e configurará a propriedade *isVerified* como *true*.

4. [Indicar](../api/domain-update.md) os serviços com suporte que você planeja usar com o domínio.

5. [Configurar](../api/domain-list-serviceconfigurationrecords.md) serviços como suporte para recuperar uma lista de registros necessários para ativar os serviços para o domínio. Adicione os detalhes de registro de configuração ao arquivo de zona do domínio usando o registrador de domínio ou a configuração do servidor DNS.

## <a name="methods"></a>Métodos

| Método   | Tipo de retorno |Descrição|
|:---------------|:--------|:----------|
|[Obter domínio](../api/domain-get.md) | [domain](domain.md) | Leia as propriedades e os relacionamentos de um objeto de domínio.|
|[Criar domínio](../api/domain-post-domains.md) | [domain](domain.md) | Adiciona um domínio ao inquilino. |
|[List domainNameReference](../api/domain-list-domainnamereferences.md) |Coleção [directoryObject](directoryobject.md)| Recupere uma lista de objetos de diretório com uma referência ao domínio.|
|[List serviceConfigurationRecords](../api/domain-list-serviceconfigurationrecords.md) |Coleção [domainDnsRecord](domaindnsrecord.md)|  Recupere uma lista dos registros DNS do domínio para configuração de domínio.|
|[List verificationDnsRecords](../api/domain-list-verificationdnsrecords.md) |Coleção [domainDnsRecord](domaindnsrecord.md)|  Recupere uma lista dos registros DNS do domínio para verificação de domínio.|
|[Atualizar domínio](../api/domain-update.md) | [domain](domain.md) |Atualiza um domínio.|
|[Excluir domínio](../api/domain-delete.md) | Nenhum |Exclui um domínio.|
|[Domínio ForceDelete](../api/domain-forcedelete.md)|Nenhum|Exclui um domínio usando uma operação assíncrona.|
|[Verificar domínio](../api/domain-verify.md)|[domain](domain.md)|Valida a propriedade do domínio.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo | Descrição |
|:---------------|:--------|:----------|
|authenticationType|String| Indica o tipo de autenticação configurado para o domínio. O valor será *Gerenciado* ou *Federado*.<br> *Gerenciado* indica um domínio gerenciado em nuvem, no qual o Azure AD realiza autenticação do usuário.<br>*Federada* indica que a autenticação é federada com um provedor de identidade como o Active Directory do locatário no local pelos Serviços de Federação do Active Directory. Não anulável |
|availabilityStatus|String| Essa propriedade é sempre nula, exceto quando a ação [verify](../api/domain-verify.md) é usada. Quando a ação [verify](../api/domain-verify.md) é usada, uma entidade **domain** é retornada na resposta. A propriedade **availabilityStatus** da entidade **domain** na resposta é *AvailableImmediately* ou *EmailVerifiedDomainTakeoverScheduled*.|
|id|String| O nome totalmente qualificado do domínio. Chave, imutável, não anulável, exclusivo |
|isAdminManaged|Booliano| O valor da propriedade será false se o gerenciamento de registro DNS do domínio foi delegado para o Office 365. Caso contrário, o valor é verdadeiro. Não anulável |
|isDefault|Booliano| True se este é o domínio padrão usado para a criação de usuário. Há apenas um domínio padrão por empresa. Não anulável |
|isInitial|Booliano| True se este é o domínio inicial criado pelo Microsoft Online Services (nomedaempresa.onmicrosoft.com). Há apenas um domínio inicial por empresa. Não anulável |
|isRoot|Booliano| True se o domínio é um domínio raiz verificado. Caso contrário, false se o domínio é um subdomínio ou não verificado. Não anulável |
|isVerified|Booliano| True se o domínio tiver concluído a verificação de propriedade de domínio. Não anulável |
|supportedServices|Coleção de cadeias de caracteres| Os recursos atribuídos ao domínio.<br><br>Podem incluir 0, 1 ou mais dos seguintes valores: *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*<br><br> Os valores que você pode adicionar ou remover usando a API do Graph incluem: *Email*, *OfficeCommunicationsOnline*, *Yammer*<br>Não anulável|
|estado|[domainState](domainstate.md)| Status de operações assíncronas agendadas em um domínio. |

## <a name="relationships"></a>Relações

As relações entre um domínio e outros objetos no diretório como seus registros de verificação e de configuração de serviço expostas por meio de propriedades de navegação. Você pode ler essas relações ao direcionar essas propriedades de navegação em suas solicitações.

| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|domainNameReferences|Coleção [directoryObject](directoryobject.md)| Somente leitura, Anulável|
|serviceConfigurationRecords|Coleção [domainDnsRecord](domaindnsrecord.md)| Os registros DNS que o cliente adiciona ao arquivo de zona DNS do domínio antes que o domínio possa ser usado pelo Microsoft Online Services.<br>Somente leitura, Anulável |
|verificationDnsRecords|Coleção [domainDnsRecord](domaindnsrecord.md)| Os registros DNS que o cliente adiciona ao arquivo de zona DNS do domínio para que o cliente possa concluir a verificação de propriedade de domínio com o Azure AD.<br>Somente leitura, Anulável|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
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
  "state": {"@odata.type": "microsoft.graph.domainState"},
  "supportedServices": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
