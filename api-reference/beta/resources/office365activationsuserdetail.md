---
title: tipo de recurso office365ActivationsUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 45219f7666d4432bcdb2b409491338b94650a726
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522474"
---
# <a name="office365activationsuserdetail-resource-type"></a><span data-ttu-id="db843-103">tipo de recurso office365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="db843-103">office365ActivationsUserDetail resource type</span></span>

<span data-ttu-id="db843-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="db843-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="db843-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db843-105">Properties</span></span>

| <span data-ttu-id="db843-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db843-106">Property</span></span>             | <span data-ttu-id="db843-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="db843-107">Type</span></span>                                     | <span data-ttu-id="db843-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="db843-108">Description</span></span>                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| <span data-ttu-id="db843-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="db843-109">reportRefreshDate</span></span>    | <span data-ttu-id="db843-110">Data</span><span class="sxs-lookup"><span data-stu-id="db843-110">Date</span></span>                                     | <span data-ttu-id="db843-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="db843-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="db843-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="db843-112">userPrincipalName</span></span>    | <span data-ttu-id="db843-113">String</span><span class="sxs-lookup"><span data-stu-id="db843-113">String</span></span>                                   | <span data-ttu-id="db843-114">O nome UPN do usuário.</span><span class="sxs-lookup"><span data-stu-id="db843-114">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="db843-115">O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet.</span><span class="sxs-lookup"><span data-stu-id="db843-115">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="db843-116">Por convenção, ele deve ser mapeado para o nome de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="db843-116">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="db843-117">O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário.</span><span class="sxs-lookup"><span data-stu-id="db843-117">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="db843-118">Essa propriedade é obrigatória quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="db843-118">This property is required when a user is created.</span></span> |
| <span data-ttu-id="db843-119">displayName</span><span class="sxs-lookup"><span data-stu-id="db843-119">displayName</span></span>          | <span data-ttu-id="db843-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db843-120">String</span></span>                                   | <span data-ttu-id="db843-121">O nome exibido para o usuário no catálogo de endereços.</span><span class="sxs-lookup"><span data-stu-id="db843-121">The name displayed in the address book for the user.</span></span> <span data-ttu-id="db843-122">Geralmente é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="db843-122">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="db843-123">Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações.</span><span class="sxs-lookup"><span data-stu-id="db843-123">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="db843-124">userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="db843-124">userActivationCounts</span></span> | <span data-ttu-id="db843-125">coleção [userActivationCounts](../resources/useractivationcounts.md)</span><span class="sxs-lookup"><span data-stu-id="db843-125">[userActivationCounts](../resources/useractivationcounts.md) collection</span></span> | <span data-ttu-id="db843-126">A ativação do produto mais recente do usuário conta com todas as plataformas para todos os tipos de produtos atribuídos.</span><span class="sxs-lookup"><span data-stu-id="db843-126">The user's latest product activation counts on all the platforms for all the assigned product types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="db843-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db843-127">JSON representation</span></span>

<span data-ttu-id="db843-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db843-128">The following is a JSON representation of the resource.</span></span>

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
