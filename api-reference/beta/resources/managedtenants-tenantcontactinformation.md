---
title: Tipo de recurso tenantContactInformation
description: Representa um contato em um locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: b60005cf60a9ac1b96a3b650a853f8b198d27e48
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402138"
---
# <a name="tenantcontactinformation-resource-type"></a><span data-ttu-id="2fd58-103">Tipo de recurso tenantContactInformation</span><span class="sxs-lookup"><span data-stu-id="2fd58-103">tenantContactInformation resource type</span></span>

<span data-ttu-id="2fd58-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="2fd58-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fd58-105">Representa um contato em um locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="2fd58-105">Represents a contact at a managed tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="2fd58-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2fd58-106">Properties</span></span>
|<span data-ttu-id="2fd58-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fd58-107">Property</span></span>|<span data-ttu-id="2fd58-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fd58-108">Type</span></span>|<span data-ttu-id="2fd58-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fd58-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fd58-110">email</span><span class="sxs-lookup"><span data-stu-id="2fd58-110">email</span></span>|<span data-ttu-id="2fd58-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fd58-111">String</span></span>|<span data-ttu-id="2fd58-112">O endereço de email do contato.</span><span class="sxs-lookup"><span data-stu-id="2fd58-112">The email address for the contact.</span></span> <span data-ttu-id="2fd58-113">Opcional</span><span class="sxs-lookup"><span data-stu-id="2fd58-113">Optional</span></span>|
|<span data-ttu-id="2fd58-114">nome</span><span class="sxs-lookup"><span data-stu-id="2fd58-114">name</span></span>|<span data-ttu-id="2fd58-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fd58-115">String</span></span>|<span data-ttu-id="2fd58-116">O nome do contato.</span><span class="sxs-lookup"><span data-stu-id="2fd58-116">The name for the contact.</span></span> <span data-ttu-id="2fd58-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fd58-117">Required.</span></span>|
|<span data-ttu-id="2fd58-118">notes</span><span class="sxs-lookup"><span data-stu-id="2fd58-118">notes</span></span>|<span data-ttu-id="2fd58-119">String</span><span class="sxs-lookup"><span data-stu-id="2fd58-119">String</span></span>|<span data-ttu-id="2fd58-120">As anotações associadas ao contato.</span><span class="sxs-lookup"><span data-stu-id="2fd58-120">The notes associated with the contact.</span></span> <span data-ttu-id="2fd58-121">Opcional</span><span class="sxs-lookup"><span data-stu-id="2fd58-121">Optional</span></span>|
|<span data-ttu-id="2fd58-122">phone</span><span class="sxs-lookup"><span data-stu-id="2fd58-122">phone</span></span>|<span data-ttu-id="2fd58-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fd58-123">String</span></span>|<span data-ttu-id="2fd58-124">O número de telefone do contato.</span><span class="sxs-lookup"><span data-stu-id="2fd58-124">The phone number for the contact.</span></span> <span data-ttu-id="2fd58-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2fd58-125">Optional.</span></span>|
|<span data-ttu-id="2fd58-126">title</span><span class="sxs-lookup"><span data-stu-id="2fd58-126">title</span></span>|<span data-ttu-id="2fd58-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fd58-127">String</span></span>|<span data-ttu-id="2fd58-128">O título do contato.</span><span class="sxs-lookup"><span data-stu-id="2fd58-128">The title for the contact.</span></span> <span data-ttu-id="2fd58-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fd58-129">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fd58-130">Relações</span><span class="sxs-lookup"><span data-stu-id="2fd58-130">Relationships</span></span>
<span data-ttu-id="2fd58-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2fd58-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2fd58-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2fd58-132">JSON representation</span></span>
<span data-ttu-id="2fd58-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2fd58-133">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantContactInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantContactInformation",
  "name": "String",
  "title": "String",
  "email": "String",
  "phone": "String",
  "notes": "String"
}
```
