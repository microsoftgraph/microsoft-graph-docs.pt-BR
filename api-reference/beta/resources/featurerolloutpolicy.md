---
title: Tipo de recurso featureRolloutPolicy
description: Representa uma política de lançamento de recursos associada a um objeto de diretório.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fa572cf9140a00d28b9db9d0e6a8e58fe6bb8969
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161667"
---
# <a name="featurerolloutpolicy-resource-type"></a>Tipo de recurso featureRolloutPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política de lançamento de recursos associada a um objeto de diretório. A criação de uma política de lançamento de recursos ajuda os administradores de locatários a controlar recursos do Azure AD com um grupo específico antes de ativar recursos para toda a organização. Isso minimiza o impacto e ajuda os administradores a testar e lançar gradualmente os recursos relacionados à autenticação.

A seguir estão as limitações da lançamento de recursos:

- Cada recurso oferece suporte a no máximo 10 grupos.
- O **campo appliesTo** só oferece suporte a grupos.
- Grupos dinâmicos e grupos aninhados não são suportados.

A seguir estão os pré-requisitos para cada um dos recursos atualmente com suporte para a lançamento usando essa política de lançamento.

### <a name="passthrough-authentication"></a>Autenticação de passagem

* Identifique um servidor executando o Windows Server 2012 R2 ou posterior onde você deseja que o [Agente PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) seja executado.Verifique se o servidor está ingressado no domínio, se pode autenticar usuários selecionados no Active Directory e se pode se comunicar com o Azure AD em portas de saída/URLs.
* [Baixe](https://aka.ms/getauthagent) & instalar o Agente de Autenticação do Microsoft Azure AD Connect no servidor.
* Para habilitar a alta disponibilidade, instale agentes de autenticação adicionais em outros servidores, conforme descrito [aqui.](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability)
* Verifique se você definiu as [configurações de Bloqueio](/azure/active-directory/authentication/howto-password-smart-lockout) Inteligente adequadamente. Isso é para garantir que as contas do Active Directory local dos usuários não recebam o bloqueado por atores ruins.

### <a name="seamlesssso"></a>SeamlessSso

* [Habilita o SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) para as florestas do AD com base [nessas](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) instruções.

### <a name="passwordhashsync"></a>PasswordHashSync

*  [Habilita PasswordHashSync](/azure/active-directory/hybrid/whatis-phs)na página   "Recursos opcionais" no Azure AD Connect.

### <a name="emailasalternateid"></a>EmailAsAlternateId

* Associar email alternativo a contas de usuário.

## <a name="methods"></a>Métodos

| Método                                                                         | Tipo de retorno                                     | Descrição                                                               |
|:-------------------------------------------------------------------------------|:------------------------------------------------|:--------------------------------------------------------------------------|
| [Listar featureRolloutPolicies](../api/directory-list-featurerolloutpolicies.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Recupere uma lista de objetos featureRolloutPolicy.                          |
| [Obter featureRolloutPolicy](../api/featurerolloutpolicy-get.md)                 | [featureRolloutPolicy](featurerolloutpolicy.md) | Recupere as propriedades e os relacionamentos do objeto featurerolloutpolicy. |
| [Criar featureRolloutPolicy](../api/directory-post-featurerolloutpolicies.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Criar um novo objeto featureRolloutPolicy.                                 |
| [Atualizar featureRolloutPolicy](../api/featurerolloutpolicy-update.md)           | [featureRolloutPolicy](featurerolloutpolicy.md) | Atualizar as propriedades do objeto featurerolloutpolicy.                     |
| [Excluir featureRolloutPolicy](../api/featurerolloutpolicy-delete.md)           | Nenhum(a)                                            | Exclua um objeto featureRolloutPolicy.                                     |
| [Assign appliesTo](../api/featurerolloutpolicy-post-appliesto.md)              | [directoryObject](directoryobject.md)           | Atribua um directoryObject ao lançamento de recursos.                              |
| [Remover appliesTo](../api/featurerolloutpolicy-delete-appliesto.md)            | Nenhum(a)                                            | Remova um directoryObject do lançamento de recursos.                            |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|String|Uma descrição para essa política de lançamento de recursos.|
|displayName|String|O nome de exibição dessa política de lançamento de recursos.|
|recurso|stagedFeatureName| Os valores possíveis são: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.|
|id|String| Somente leitura.|
|isAppliedToOrganization|Boolean|Indica se essa política de lançamento de recursos deve ser aplicada a toda a organização.|
|isEnabled|Booliano|Indica se a lançamento de recursos está habilitada.|

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


