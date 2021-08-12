---
title: Tipo de recurso featureRolloutPolicy
description: Representa uma política de lançamento de recursos associada a um objeto de diretório.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 517ee0b3b24b7bde2e651aff704b729798da64a75f3377990c87df2be84f3cec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146871"
---
# <a name="featurerolloutpolicy-resource-type"></a>Tipo de recurso featureRolloutPolicy

Namespace: microsoft.graph

Representa uma política de lançamento de recursos associada a um objeto de diretório. A criação de uma política de lançamento de recursos ajuda os administradores de locatários a criar recursos piloto do Azure AD com um grupo específico antes de habilenciar recursos para toda a organização. Isso minimiza o impacto e ajuda os administradores a testar e lançar gradualmente os recursos relacionados à autenticação.

Veja a seguir as limitações da adoção de recursos:

- Cada recurso oferece suporte a no máximo 10 grupos.
- O **campo appliesTo só** dá suporte a grupos.
- Não há suporte para grupos dinâmicos e grupos aninhados.

A seguir estão os pré-requisitos para cada um dos recursos atualmente suportados para a adoção usando essa política de lançamento.

### <a name="passthrough-authentication"></a>Autenticação passo a passo

* Identifique um servidor executando Windows Server 2012 R2 ou posterior onde você deseja que o [Agente PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) seja executado.Verifique se o servidor está ingressado no domínio, pode autenticar usuários selecionados com o Active Directory e pode se comunicar com o Azure AD em portas de saída/URLs.
* [Baixe](https://aka.ms/getauthagent) & instalar o Microsoft Azure AD Conexão autenticação no servidor.
* Para habilitar alta disponibilidade, instale agentes de autenticação adicionais em outros servidores conforme descrito [aqui](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).
* Verifique se você configurou suas [configurações de Bloqueio](/azure/active-directory/authentication/howto-password-smart-lockout) Inteligente adequadamente. Isso é para garantir que as contas locais do Active Directory de seus usuários não são bloqueadas por atores ruins.

### <a name="seamlesssso"></a>SeamlessSso

* [Habilita o SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) para as florestas do AD com base [nessas](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) instruções.

### <a name="passwordhashsync"></a>PasswordHashSync

*  [Habilitar PasswordHashSync](/azure/active-directory/hybrid/whatis-phs)na página   "Recursos opcionais" no Azure AD Conexão.

### <a name="emailasalternateid"></a>EmailAsAlternateId

* Associe emails alternativos a contas de usuário.

## <a name="methods"></a>Métodos

| Método                                                                         | Tipo de retorno                                     | Descrição                                                               |
|:-------------------------------------------------------------------------------|:------------------------------------------------|:--------------------------------------------------------------------------|
| [Listar featureRolloutPolicies](../api/featurerolloutpolicies-list.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Recupere uma lista de objetos featureRolloutPolicy.                          |
| [Obter featureRolloutPolicy](../api/featurerolloutpolicy-get.md)                 | [featureRolloutPolicy](featurerolloutpolicy.md) | Recupere as propriedades e as relações do objeto featurerolloutpolicy. |
| [Criar featureRolloutPolicy](../api/featurerolloutpolicies-post.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Crie um novo objeto featureRolloutPolicy.                                 |
| [Atualizar featureRolloutPolicy](../api/featurerolloutpolicy-update.md)           | [featureRolloutPolicy](featurerolloutpolicy.md) | Atualize as propriedades do objeto featurerolloutpolicy.                     |
| [Excluir featureRolloutPolicy](../api/featurerolloutpolicy-delete.md)           | None                                            | Exclua um objeto featureRolloutPolicy.                                     |
| [Atribuir appliesTo](../api/featurerolloutpolicy-post-appliesto.md)              | [directoryObject](directoryobject.md)           | Atribua um directoryObject à atribuição de recursos.                              |
| [Remover appliesTo](../api/featurerolloutpolicy-delete-appliesto.md)            | None                                            | Remover um directoryObject da adoção de recursos.                            |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|Cadeia de caracteres|Uma descrição para essa política de lançamento de recursos.|
|displayName|String|O nome de exibição dessa política de lançamento de recursos.|
|feature|stagedFeatureName| Os valores possíveis são: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `emailAsAlternateId`, `unknownFutureValue`.|
|id|String| Somente leitura.|
|isAppliedToOrganization|Booliano|Indica se essa política de lançamento de recursos deve ser aplicada a toda a organização.|
|isEnabled|Booliano|Indica se a adoção de recursos está habilitada.|

### <a name="stagedfeaturename-values"></a>valores stagedFeatureName 

|Member|
|:---|
|passthroughAuthentication|
|seamlessSso|
|passwordHashSync|
|emailAsAlternateId|
|unknownFutureValue|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|appliesTo|Coleção [directoryObject](directoryobject.md)| Anulável. Especifica uma lista de directoryObjects para os qual o recurso está habilitado.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "feature": "string",
  "id": "String (identifier)",
  "isAppliedToOrganization": false,
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "featureRolloutPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


