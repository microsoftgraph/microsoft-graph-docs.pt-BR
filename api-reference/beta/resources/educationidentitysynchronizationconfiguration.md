    ---
title: "tipo de recurso educationIdentitySynchronizationConfiguration" Descrição: "classe abstrata base para todas as configurações de sincronização de identidade de perfil de dados da escola. As classes derivadas definem o comportamento da sincronização de identidades. Estes são os tipos derivados. "
Author: "mmast-MSFT" localization_priority: normal MS. Prod: "educação"
---

# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>tipo de recurso educationIdentitySynchronizationConfiguration

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Classe abstrata de base para todas as configurações de sincronização de identidade de perfil de dados da escola. As classes derivadas definem o comportamento da sincronização de identidades. Estes são os tipos derivados.

## <a name="derived-types"></a>Tipos derivados
| Tipo | Descrição |
|:-|:-|
| [**educationIdentityMatchingConfiguration**](educationidentitymatchingconfiguration.md) | Use este tipo para fazer a correspondência de contas de usuário existentes no Azure Active Directory (Azure AD). |
| [**educationIdentityCreationConfiguration**](educationidentitycreationconfiguration.md) | Use este tipo para criar novas contas de usuário no Azure AD. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitysynchronizationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
