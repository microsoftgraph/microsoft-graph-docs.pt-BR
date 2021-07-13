---
title: Tipo de recurso tenantContract
description: Representa as informações de relação entre um locatário e a entidade de gerenciamento.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 104b475428efe82a2e56f823845b933149aeab18
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401995"
---
# <a name="tenantcontract-resource-type"></a><span data-ttu-id="f1986-103">Tipo de recurso tenantContract</span><span class="sxs-lookup"><span data-stu-id="f1986-103">tenantContract resource type</span></span>

<span data-ttu-id="f1986-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="f1986-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1986-105">Representa as informações de relação entre um locatário e a entidade de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f1986-105">Represents relationship information between a tenant and the managing entity.</span></span>

## <a name="properties"></a><span data-ttu-id="f1986-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1986-106">Properties</span></span>
|<span data-ttu-id="f1986-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1986-107">Property</span></span>|<span data-ttu-id="f1986-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1986-108">Type</span></span>|<span data-ttu-id="f1986-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1986-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1986-110">contractType</span><span class="sxs-lookup"><span data-stu-id="f1986-110">contractType</span></span>|<span data-ttu-id="f1986-111">Int32</span><span class="sxs-lookup"><span data-stu-id="f1986-111">Int32</span></span>|<span data-ttu-id="f1986-112">O tipo de relação existente entre a entidade de gerenciamento e o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1986-112">The type of relationship that exists between the managing entity and tenant.</span></span> <span data-ttu-id="f1986-113">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f1986-113">Optional.</span></span> <span data-ttu-id="f1986-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1986-114">Read-only.</span></span>|
|<span data-ttu-id="f1986-115">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="f1986-115">defaultDomainName</span></span>|<span data-ttu-id="f1986-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1986-116">String</span></span>|<span data-ttu-id="f1986-117">O nome de domínio padrão para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1986-117">The default domain name for the tenant.</span></span> <span data-ttu-id="f1986-118">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1986-118">Required.</span></span> <span data-ttu-id="f1986-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1986-119">Read-only.</span></span>|
|<span data-ttu-id="f1986-120">displayName</span><span class="sxs-lookup"><span data-stu-id="f1986-120">displayName</span></span>|<span data-ttu-id="f1986-121">String</span><span class="sxs-lookup"><span data-stu-id="f1986-121">String</span></span>|<span data-ttu-id="f1986-122">O nome de exibição do locatário.</span><span class="sxs-lookup"><span data-stu-id="f1986-122">The display name for the tenant.</span></span> <span data-ttu-id="f1986-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f1986-123">Optional.</span></span> <span data-ttu-id="f1986-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1986-124">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1986-125">Relações</span><span class="sxs-lookup"><span data-stu-id="f1986-125">Relationships</span></span>
<span data-ttu-id="f1986-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f1986-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1986-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1986-127">JSON representation</span></span>
<span data-ttu-id="f1986-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1986-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantContract"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantContract",
  "contractType": "Integer",
  "displayName": "String",
  "defaultDomainName": "String"
}
```
