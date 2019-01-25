    ---
título: "tipo de recurso de educationIdentitySynchronizationConfiguration" Descrição: "classe abstrata base para configurações de sincronização de identidade de perfil do escola dados todos. As classes derivadas definem o comportamento para sincronização de identidades. A seguir estão os tipos derivados."
autor: "mmast-msft" localization_priority: ms.prod Normal: "educação"
---

# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>tipo de recurso de educationIdentitySynchronizationConfiguration

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Classe base abstrata para todas as escola dados perfil identidade sincronização configurações. As classes derivadas definem o comportamento para sincronização de identidades. A seguir estão os tipos derivados.

## <a name="derived-types"></a>Tipos derivados
| Tipo | Descrição |
|:-|:-|
| [**educationIdentityMatchingConfiguration**](educationidentitymatchingconfiguration.md) | Use este tipo para corresponder as contas de usuário existentes no Windows Azure Active Directory (AD Azure). |
| [**educationIdentityCreationConfiguration**](educationidentitycreationconfiguration.md) | Use este tipo para criar novas contas de usuário no Azure AD. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitysynchronizationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
