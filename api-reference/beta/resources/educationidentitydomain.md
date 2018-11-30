---
title: tipo de recurso de educationIdentityDomain
description: 'Representa o mapeamento entre um tipo de usuário de educação e o domínio em que a conta do usuário pertence. O recurso de domínio é parte da configuração de criação de identidade. '
ms.openlocfilehash: 8298e1eb38ae70f982719ee3a7d6588cd181bdd8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038347"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="693c7-104">tipo de recurso de educationIdentityDomain</span><span class="sxs-lookup"><span data-stu-id="693c7-104">educationIdentityDomain resource type</span></span>

> <span data-ttu-id="693c7-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="693c7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="693c7-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="693c7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="693c7-107">Representa o mapeamento entre um tipo de usuário de educação e o domínio em que a conta do usuário pertence.</span><span class="sxs-lookup"><span data-stu-id="693c7-107">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="693c7-108">O recurso de domínio é parte da [configuração de criação de identidade](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="693c7-108">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="693c7-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="693c7-109">Properties</span></span>

| <span data-ttu-id="693c7-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="693c7-110">Property</span></span> | <span data-ttu-id="693c7-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="693c7-111">Type</span></span> | <span data-ttu-id="693c7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="693c7-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="693c7-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="693c7-113">**appliesTo**</span></span> | <span data-ttu-id="693c7-114">string</span><span class="sxs-lookup"><span data-stu-id="693c7-114">string</span></span> |  <span data-ttu-id="693c7-115">O tipo de função de usuário para atribuir a licença.</span><span class="sxs-lookup"><span data-stu-id="693c7-115">The user role type to assign to license.</span></span> <span data-ttu-id="693c7-116">Os valores possíveis são: `student` e `teacher`.</span><span class="sxs-lookup"><span data-stu-id="693c7-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="693c7-117">**name**</span><span class="sxs-lookup"><span data-stu-id="693c7-117">**name**</span></span> | <span data-ttu-id="693c7-118">string</span><span class="sxs-lookup"><span data-stu-id="693c7-118">string</span></span> |  <span data-ttu-id="693c7-119">Representa o domínio da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="693c7-119">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="693c7-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="693c7-120">JSON representation</span></span>
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
