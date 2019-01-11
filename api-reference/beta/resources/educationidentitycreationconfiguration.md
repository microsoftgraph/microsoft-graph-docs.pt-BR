---
title: tipo de recurso de educationIdentityCreationConfiguration
description: Define as configurações na criação das identidades de perfil de dados escola. Essas identidades incluem alunos e professores. Com base nessas configurações, os usuários serão criados no diretório.
localization_priority: Normal
ms.openlocfilehash: 86624c7203dc6425372556572c40efda2bc1a53f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858860"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="c06c9-105">tipo de recurso de educationIdentityCreationConfiguration</span><span class="sxs-lookup"><span data-stu-id="c06c9-105">educationIdentityCreationConfiguration resource type</span></span>

> <span data-ttu-id="c06c9-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c06c9-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c06c9-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c06c9-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c06c9-108">Define as configurações na criação das identidades de perfil de dados escola.</span><span class="sxs-lookup"><span data-stu-id="c06c9-108">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="c06c9-109">Essas identidades incluem alunos e professores.</span><span class="sxs-lookup"><span data-stu-id="c06c9-109">These identities include students and teachers.</span></span> <span data-ttu-id="c06c9-110">Com base nessas configurações, os usuários serão criados no diretório.</span><span class="sxs-lookup"><span data-stu-id="c06c9-110">Based on these settings, the users will be created in the directory.</span></span>

> <span data-ttu-id="c06c9-111">**Observação:** Se você tiver ativada a sincronização entre o local do Active Directory e o Azure Active Directory (AD Azure) de sincronização de diretório, use o recurso de [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c06c9-111">**Note:** If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="c06c9-112">Derivado do [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c06c9-112">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c06c9-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c06c9-113">Properties</span></span>

| <span data-ttu-id="c06c9-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c06c9-114">Property</span></span> | <span data-ttu-id="c06c9-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="c06c9-115">Type</span></span> | <span data-ttu-id="c06c9-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="c06c9-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="c06c9-117">**userDomains**</span><span class="sxs-lookup"><span data-stu-id="c06c9-117">**userDomains**</span></span> | <span data-ttu-id="c06c9-118">coleção [educationIdentityDomain](educationidentitydomain.md)</span><span class="sxs-lookup"><span data-stu-id="c06c9-118">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> |  <span data-ttu-id="c06c9-119">Define a lista de domínios a serem utilizadas por tipo de usuário.</span><span class="sxs-lookup"><span data-stu-id="c06c9-119">Sets the list of domains to use per user type.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="c06c9-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c06c9-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "#microsoft.graph.educationIdentityDomain",
        }
    ]
}
```
