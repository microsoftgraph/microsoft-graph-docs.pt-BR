    ---
<span data-ttu-id="a9aad-101">título: "tipo de recurso de educationIdentitySynchronizationConfiguration" Descrição: "classe abstrata base para configurações de sincronização de identidade de perfil do escola dados todos.</span><span class="sxs-lookup"><span data-stu-id="a9aad-101">title: "educationIdentitySynchronizationConfiguration resource type" description: "Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="a9aad-102">As classes derivadas definem o comportamento para sincronização de identidades.</span><span class="sxs-lookup"><span data-stu-id="a9aad-102">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="a9aad-103">A seguir estão os tipos derivados."</span><span class="sxs-lookup"><span data-stu-id="a9aad-103">The following are the derived types."</span></span>
<span data-ttu-id="a9aad-104">autor: "mmast-msft" localization_priority: ms.prod Normal: "educação"</span><span class="sxs-lookup"><span data-stu-id="a9aad-104">author: "mmast-msft" localization_priority: Normal ms.prod: "education"</span></span>
---

# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="a9aad-105">tipo de recurso de educationIdentitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a9aad-105">educationIdentitySynchronizationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9aad-106">Classe base abstrata para todas as escola dados perfil identidade sincronização configurações.</span><span class="sxs-lookup"><span data-stu-id="a9aad-106">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="a9aad-107">As classes derivadas definem o comportamento para sincronização de identidades.</span><span class="sxs-lookup"><span data-stu-id="a9aad-107">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="a9aad-108">A seguir estão os tipos derivados.</span><span class="sxs-lookup"><span data-stu-id="a9aad-108">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="a9aad-109">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="a9aad-109">Derived types</span></span>
| <span data-ttu-id="a9aad-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9aad-110">Type</span></span> | <span data-ttu-id="a9aad-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9aad-111">Description</span></span> |
|:-|:-|
| [<span data-ttu-id="a9aad-112">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="a9aad-112">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="a9aad-113">Use este tipo para corresponder as contas de usuário existentes no Windows Azure Active Directory (AD Azure).</span><span class="sxs-lookup"><span data-stu-id="a9aad-113">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="a9aad-114">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="a9aad-114">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="a9aad-115">Use este tipo para criar novas contas de usuário no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a9aad-115">Use this type to create new user accounts in Azure AD.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitysynchronizationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
