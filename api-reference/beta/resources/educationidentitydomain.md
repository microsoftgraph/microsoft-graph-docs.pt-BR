---
title: tipo de recurso de educationIdentityDomain
description: 'Representa o mapeamento entre um tipo de usuário de educação e o domínio em que a conta do usuário pertence. O recurso de domínio é parte da configuração de criação de identidade. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 280ae1a65e0c14e7960d316cc21154e405f2ee0d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982026"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="12d61-104">tipo de recurso de educationIdentityDomain</span><span class="sxs-lookup"><span data-stu-id="12d61-104">educationIdentityDomain resource type</span></span>

> <span data-ttu-id="12d61-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="12d61-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12d61-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="12d61-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12d61-107">Representa o mapeamento entre um tipo de usuário de educação e o domínio em que a conta do usuário pertence.</span><span class="sxs-lookup"><span data-stu-id="12d61-107">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="12d61-108">O recurso de domínio é parte da [configuração de criação de identidade](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12d61-108">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="12d61-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12d61-109">Properties</span></span>

| <span data-ttu-id="12d61-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12d61-110">Property</span></span> | <span data-ttu-id="12d61-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="12d61-111">Type</span></span> | <span data-ttu-id="12d61-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="12d61-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="12d61-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="12d61-113">**appliesTo**</span></span> | <span data-ttu-id="12d61-114">string</span><span class="sxs-lookup"><span data-stu-id="12d61-114">string</span></span> |  <span data-ttu-id="12d61-115">O tipo de função de usuário para atribuir a licença.</span><span class="sxs-lookup"><span data-stu-id="12d61-115">The user role type to assign to license.</span></span> <span data-ttu-id="12d61-116">Os valores possíveis são: `student` e `teacher`.</span><span class="sxs-lookup"><span data-stu-id="12d61-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="12d61-117">**name**</span><span class="sxs-lookup"><span data-stu-id="12d61-117">**name**</span></span> | <span data-ttu-id="12d61-118">string</span><span class="sxs-lookup"><span data-stu-id="12d61-118">string</span></span> |  <span data-ttu-id="12d61-119">Representa o domínio da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="12d61-119">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="12d61-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12d61-120">JSON representation</span></span>
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
