    ---
<span data-ttu-id="f2132-101">title: "tipo de recurso educationIdentitySynchronizationConfiguration" Descrição: "classe abstrata base para todas as configurações de sincronização de identidade de perfil de dados da escola.</span><span class="sxs-lookup"><span data-stu-id="f2132-101">title: "educationIdentitySynchronizationConfiguration resource type" description: "Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="f2132-102">As classes derivadas definem o comportamento da sincronização de identidades.</span><span class="sxs-lookup"><span data-stu-id="f2132-102">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="f2132-103">Estes são os tipos derivados. "</span><span class="sxs-lookup"><span data-stu-id="f2132-103">The following are the derived types."</span></span>
<span data-ttu-id="f2132-104">Author: "mmast-MSFT" localization_priority: normal MS. Prod: "educação"</span><span class="sxs-lookup"><span data-stu-id="f2132-104">author: "mmast-msft" localization_priority: Normal ms.prod: "education"</span></span>
---

# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="f2132-105">tipo de recurso educationIdentitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2132-105">educationIdentitySynchronizationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2132-106">Classe abstrata de base para todas as configurações de sincronização de identidade de perfil de dados da escola.</span><span class="sxs-lookup"><span data-stu-id="f2132-106">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="f2132-107">As classes derivadas definem o comportamento da sincronização de identidades.</span><span class="sxs-lookup"><span data-stu-id="f2132-107">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="f2132-108">Estes são os tipos derivados.</span><span class="sxs-lookup"><span data-stu-id="f2132-108">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="f2132-109">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="f2132-109">Derived types</span></span>
| <span data-ttu-id="f2132-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2132-110">Type</span></span> | <span data-ttu-id="f2132-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2132-111">Description</span></span> |
|:-|:-|
| [<span data-ttu-id="f2132-112">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="f2132-112">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="f2132-113">Use este tipo para fazer a correspondência de contas de usuário existentes no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="f2132-113">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="f2132-114">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="f2132-114">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="f2132-115">Use este tipo para criar novas contas de usuário no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f2132-115">Use this type to create new user accounts in Azure AD.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitysynchronizationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
