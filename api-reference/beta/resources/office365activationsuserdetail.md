---
title: tipo de recurso de office365ActivationsUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 3e2b7d5fb3c42db02407a187649544b2560f898a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982852"
---
# <a name="office365activationsuserdetail-resource-type"></a><span data-ttu-id="604ea-103">tipo de recurso de office365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="604ea-103">office365ActivationsUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="604ea-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="604ea-104">Properties</span></span>

| <span data-ttu-id="604ea-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="604ea-105">Property</span></span>             | <span data-ttu-id="604ea-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="604ea-106">Type</span></span>                                     | <span data-ttu-id="604ea-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="604ea-107">Description</span></span>                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| <span data-ttu-id="604ea-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="604ea-108">reportRefreshDate</span></span>    | <span data-ttu-id="604ea-109">Data</span><span class="sxs-lookup"><span data-stu-id="604ea-109">Date</span></span>                                     | <span data-ttu-id="604ea-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="604ea-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="604ea-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="604ea-111">userPrincipalName</span></span>    | <span data-ttu-id="604ea-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="604ea-112">String</span></span>                                   | <span data-ttu-id="604ea-113">O usuário nome principal (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="604ea-113">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="604ea-114">O UPN é um nome de logon estilo Internet para o usuário com base na Internet padrão RFC 822.</span><span class="sxs-lookup"><span data-stu-id="604ea-114">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="604ea-115">Por convenção, isso deve ser mapeada para o nome de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="604ea-115">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="604ea-116">O formato geral é alias@domain, onde o domínio deve estar presente na coleção de locatário de domínios verificados.</span><span class="sxs-lookup"><span data-stu-id="604ea-116">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="604ea-117">Essa propriedade é obrigatória quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="604ea-117">This property is required when a user is created.</span></span> |
| <span data-ttu-id="604ea-118">displayName</span><span class="sxs-lookup"><span data-stu-id="604ea-118">displayName</span></span>          | <span data-ttu-id="604ea-119">String</span><span class="sxs-lookup"><span data-stu-id="604ea-119">String</span></span>                                   | <span data-ttu-id="604ea-120">O nome exibido para o usuário no catálogo de endereços.</span><span class="sxs-lookup"><span data-stu-id="604ea-120">The name displayed in the address book for the user.</span></span> <span data-ttu-id="604ea-121">Geralmente é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="604ea-121">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="604ea-122">Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações.</span><span class="sxs-lookup"><span data-stu-id="604ea-122">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="604ea-123">userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="604ea-123">userActivationCounts</span></span> | <span data-ttu-id="604ea-124">coleção [userActivationCounts](../resources/useractivationcounts.md)</span><span class="sxs-lookup"><span data-stu-id="604ea-124">[userActivationCounts](../resources/useractivationcounts.md) collection</span></span> | <span data-ttu-id="604ea-125">Ativação do produto mais recente do usuário a contagem de todas as plataformas para todos os tipos de produto atribuído.</span><span class="sxs-lookup"><span data-stu-id="604ea-125">The user's latest product activation counts on all the platforms for all the assigned product types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="604ea-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="604ea-126">JSON representation</span></span>

<span data-ttu-id="604ea-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="604ea-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userActivationCounts": [{"@odata.type":"microsoft.graph.userActivationCounts"}]
}
```
