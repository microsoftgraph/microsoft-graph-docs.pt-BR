---
title: tipo de recurso de educationIdentityDomain
description: 'Representa o mapeamento entre um tipo de usuário de educação e o domínio em que a conta do usuário pertence. O recurso de domínio é parte da configuração de criação de identidade. '
localization_priority: Normal
ms.openlocfilehash: 5675499aca010f90deeb517210065ac4802d66b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807746"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="3ac79-104">tipo de recurso de educationIdentityDomain</span><span class="sxs-lookup"><span data-stu-id="3ac79-104">educationIdentityDomain resource type</span></span>

> <span data-ttu-id="3ac79-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3ac79-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ac79-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3ac79-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3ac79-107">Representa o mapeamento entre um tipo de usuário de educação e o domínio em que a conta do usuário pertence.</span><span class="sxs-lookup"><span data-stu-id="3ac79-107">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="3ac79-108">O recurso de domínio é parte da [configuração de criação de identidade](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3ac79-108">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="3ac79-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ac79-109">Properties</span></span>

| <span data-ttu-id="3ac79-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ac79-110">Property</span></span> | <span data-ttu-id="3ac79-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ac79-111">Type</span></span> | <span data-ttu-id="3ac79-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ac79-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="3ac79-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="3ac79-113">**appliesTo**</span></span> | <span data-ttu-id="3ac79-114">string</span><span class="sxs-lookup"><span data-stu-id="3ac79-114">string</span></span> |  <span data-ttu-id="3ac79-115">O tipo de função de usuário para atribuir a licença.</span><span class="sxs-lookup"><span data-stu-id="3ac79-115">The user role type to assign to license.</span></span> <span data-ttu-id="3ac79-116">Os valores possíveis são: `student` e `teacher`.</span><span class="sxs-lookup"><span data-stu-id="3ac79-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="3ac79-117">**name**</span><span class="sxs-lookup"><span data-stu-id="3ac79-117">**name**</span></span> | <span data-ttu-id="3ac79-118">string</span><span class="sxs-lookup"><span data-stu-id="3ac79-118">string</span></span> |  <span data-ttu-id="3ac79-119">Representa o domínio da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="3ac79-119">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="3ac79-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ac79-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "name": "String"
}
```
