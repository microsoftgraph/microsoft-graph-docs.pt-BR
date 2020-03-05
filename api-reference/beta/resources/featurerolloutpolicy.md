---
title: tipo de recurso featureRolloutPolicy
description: Representa uma política de distribuição de recursos associada a um objeto de diretório.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a5ebc5884b0fd1ccf52fca961247e610b1c8cad5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498480"
---
# <a name="featurerolloutpolicy-resource-type"></a>tipo de recurso featureRolloutPolicy

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política de distribuição de recursos associada a um objeto de diretório. A criação de uma política de distribuição de recursos ajuda os administradores de locatários a recursos piloto do Azure AD com um grupo específico antes de habilitar recursos para toda a organização. Isso minimiza o impacto e ajuda os administradores a testar e a distribuir recursos relacionados à autenticação gradualmente.

Veja a seguir as limitações da distribuição de recursos:

- Cada recurso oferece suporte a um máximo de 10 grupos.
- O campo **AppliesTo** só oferece suporte a grupos.
- Não há suporte para grupos dinâmicos e aninhados.

Estes são os requisitos para cada um dos recursos atualmente suported para distribuição usando esta política de distribuição.

### <a name="passthrough-authentication"></a>Autenticação de passagem

* Identifique um servidor executando o Windows Server 2012 R2 ou posterior onde você deseja que o agente do [PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) seja executado.Certifique-se de que o servidor ingressou no domínio, possa autenticar usuários selecionados com o Active Directory e pode se comunicar com o Azure AD em portas/URLs de saída.
* [Baixe](https://aka.ms/getauthagent) & instale o agente de autenticação do Microsoft Azure ad Connect no servidor.
* Para habilitar a alta disponibilidade, instale agentes de autenticação adicionais em outros servidores, conforme descrito [aqui](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).
* Verifique se você configurou suas configurações de [bloqueio inteligente](/azure/active-directory/authentication/howto-password-smart-lockout) adequadamente. Isso é para garantir que as contas do Active Directory no local dos usuários não sejam bloqueadas por atores ruins.

### <a name="seamlesssso"></a>SeamlessSso

* Habilite o [SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) para as florestas do AD com [base nessas instruções.](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature)

### <a name="passwordhashsync"></a>PasswordHashSync

* Habilite o [PasswordHashSync](/azure/active-directory/hybrid/whatis-phs) na página "recursos opcionais" no Azure ad Connect.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar featureRolloutPolicies](../api/directory-list-featurerolloutpolicies.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Recupere uma lista de objetos featureRolloutPolicy. |
| [Obter featureRolloutPolicy](../api/featurerolloutpolicy-get.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Recupere as propriedades e os relacionamentos do objeto featurerolloutpolicy. ||
| [Criar featureRolloutPolicy](../api/directory-post-featurerolloutpolicies.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Criar um novo objeto featureRolloutPolicy.
| [Atualizar featureRolloutPolicy](../api/featurerolloutpolicy-update.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Atualize as propriedades do objeto featurerolloutpolicy. |
| [Excluir featureRolloutPolicy](../api/featurerolloutpolicy-delete.md) | Nenhum | Excluir um objeto featureRolloutPolicy. |
| [Atribuir aplica-se](../api/featurerolloutpolicy-post-appliesto.md) | [directoryObject](directoryobject.md) | Atribua um directoryobject à distribuição de recursos. |
| [Remover aplica-se](../api/featurerolloutpolicy-delete-appliesto.md) | Nenhum | Remover um directoryobject da distribuição de recursos. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|String|Uma descrição para esta política de distribuição de recursos.|
|displayName|Cadeia de caracteres|O nome de exibição desta política de distribuição de recursos.|
|apresentam|stagedFeatureName| Os valores possíveis são: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.|
|id|String| Somente leitura.|
|isAppliedToOrganization|Boolean|Indica se esta política de distribuição de recursos deve ser aplicada a toda a organização.|
|isEnabled|Boolean|Indica se a distribuição de recursos está habilitada.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|appliesTo|Coleção [directoryObject](directoryobject.md)| Anulável. Especifica uma lista de directoryObjects para o qual o recurso está habilitado.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "baseType": "",
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
