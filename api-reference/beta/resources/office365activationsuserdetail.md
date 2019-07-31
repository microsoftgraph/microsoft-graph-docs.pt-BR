---
title: tipo de recurso office365ActivationsUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 2ced56fdc8f2ed877368163e36588e3d4983d95e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009528"
---
# <a name="office365activationsuserdetail-resource-type"></a><span data-ttu-id="f19f0-103">tipo de recurso office365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="f19f0-103">office365ActivationsUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f19f0-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f19f0-104">Properties</span></span>

| <span data-ttu-id="f19f0-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f19f0-105">Property</span></span>             | <span data-ttu-id="f19f0-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="f19f0-106">Type</span></span>                                     | <span data-ttu-id="f19f0-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="f19f0-107">Description</span></span>                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| <span data-ttu-id="f19f0-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f19f0-108">reportRefreshDate</span></span>    | <span data-ttu-id="f19f0-109">Data</span><span class="sxs-lookup"><span data-stu-id="f19f0-109">Date</span></span>                                     | <span data-ttu-id="f19f0-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f19f0-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="f19f0-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f19f0-111">userPrincipalName</span></span>    | <span data-ttu-id="f19f0-112">String</span><span class="sxs-lookup"><span data-stu-id="f19f0-112">String</span></span>                                   | <span data-ttu-id="f19f0-113">O nome UPN do usuário.</span><span class="sxs-lookup"><span data-stu-id="f19f0-113">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="f19f0-114">O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet.</span><span class="sxs-lookup"><span data-stu-id="f19f0-114">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="f19f0-115">Por convenção, ele deve ser mapeado para o nome de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="f19f0-115">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="f19f0-116">O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário.</span><span class="sxs-lookup"><span data-stu-id="f19f0-116">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="f19f0-117">Essa propriedade é obrigatória quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="f19f0-117">This property is required when a user is created.</span></span> |
| <span data-ttu-id="f19f0-118">displayName</span><span class="sxs-lookup"><span data-stu-id="f19f0-118">displayName</span></span>          | <span data-ttu-id="f19f0-119">String</span><span class="sxs-lookup"><span data-stu-id="f19f0-119">String</span></span>                                   | <span data-ttu-id="f19f0-120">O nome exibido para o usuário no catálogo de endereços.</span><span class="sxs-lookup"><span data-stu-id="f19f0-120">The name displayed in the address book for the user.</span></span> <span data-ttu-id="f19f0-121">Geralmente é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="f19f0-121">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="f19f0-122">Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações.</span><span class="sxs-lookup"><span data-stu-id="f19f0-122">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="f19f0-123">userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="f19f0-123">userActivationCounts</span></span> | <span data-ttu-id="f19f0-124">coleção [userActivationCounts](../resources/useractivationcounts.md)</span><span class="sxs-lookup"><span data-stu-id="f19f0-124">[userActivationCounts](../resources/useractivationcounts.md) collection</span></span> | <span data-ttu-id="f19f0-125">A ativação do produto mais recente do usuário conta com todas as plataformas para todos os tipos de produtos atribuídos.</span><span class="sxs-lookup"><span data-stu-id="f19f0-125">The user's latest product activation counts on all the platforms for all the assigned product types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f19f0-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f19f0-126">JSON representation</span></span>

<span data-ttu-id="f19f0-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f19f0-127">The following is a JSON representation of the resource.</span></span>

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
