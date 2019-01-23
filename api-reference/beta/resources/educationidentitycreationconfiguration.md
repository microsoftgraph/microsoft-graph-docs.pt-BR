---
title: tipo de recurso de educationIdentityCreationConfiguration
description: Define as configurações na criação das identidades de perfil de dados escola. Essas identidades incluem alunos e professores. Com base nessas configurações, os usuários serão criados no diretório.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 7c05d810c017f57f738d188a8edef5d0560415fd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395682"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="fe2d2-105">tipo de recurso de educationIdentityCreationConfiguration</span><span class="sxs-lookup"><span data-stu-id="fe2d2-105">educationIdentityCreationConfiguration resource type</span></span>

> <span data-ttu-id="fe2d2-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fe2d2-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe2d2-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fe2d2-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe2d2-108">Define as configurações na criação das identidades de perfil de dados escola.</span><span class="sxs-lookup"><span data-stu-id="fe2d2-108">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="fe2d2-109">Essas identidades incluem alunos e professores.</span><span class="sxs-lookup"><span data-stu-id="fe2d2-109">These identities include students and teachers.</span></span> <span data-ttu-id="fe2d2-110">Com base nessas configurações, os usuários serão criados no diretório.</span><span class="sxs-lookup"><span data-stu-id="fe2d2-110">Based on these settings, the users will be created in the directory.</span></span>

> <span data-ttu-id="fe2d2-111">**Observação:** Se você tiver ativada a sincronização entre o local do Active Directory e o Azure Active Directory (AD Azure) de sincronização de diretório, use o recurso de [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fe2d2-111">**Note:** If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="fe2d2-112">Derivado do [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe2d2-112">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fe2d2-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe2d2-113">Properties</span></span>

| <span data-ttu-id="fe2d2-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe2d2-114">Property</span></span> | <span data-ttu-id="fe2d2-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe2d2-115">Type</span></span> | <span data-ttu-id="fe2d2-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe2d2-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="fe2d2-117">**userDomains**</span><span class="sxs-lookup"><span data-stu-id="fe2d2-117">**userDomains**</span></span> | <span data-ttu-id="fe2d2-118">coleção [educationIdentityDomain](educationidentitydomain.md)</span><span class="sxs-lookup"><span data-stu-id="fe2d2-118">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> |  <span data-ttu-id="fe2d2-119">Define a lista de domínios a serem utilizadas por tipo de usuário.</span><span class="sxs-lookup"><span data-stu-id="fe2d2-119">Sets the list of domains to use per user type.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="fe2d2-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe2d2-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "microsoft.graph.educationIdentityDomain",
        }
    ]
}
```
