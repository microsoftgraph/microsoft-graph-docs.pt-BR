---
title: tipo de recurso relatedContact
description: Registro de contato relacionado a um educationUser que fornece informações para guardiões, auxílios, médicos e assim por diante.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 66c4329b6c81d3bad38583ccf963bb4c6bb08f50
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042405"
---
# <a name="relatedcontact-resource-type"></a><span data-ttu-id="70a6f-103">tipo de recurso relatedContact</span><span class="sxs-lookup"><span data-stu-id="70a6f-103">relatedContact resource type</span></span>

<span data-ttu-id="70a6f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70a6f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70a6f-105">Registro de contato relacionado a um [educationUser](../resources/educationuser.md) que fornece informações para guardiões, auxílios, médicos e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="70a6f-105">Contact record related to an [educationUser](../resources/educationuser.md) that provides information for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="70a6f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70a6f-106">Properties</span></span>

| <span data-ttu-id="70a6f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70a6f-107">Property</span></span>      | <span data-ttu-id="70a6f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="70a6f-108">Type</span></span>                  | <span data-ttu-id="70a6f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="70a6f-109">Description</span></span>                                                                                                         |
| :------------ | :-------------------- | :------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="70a6f-110">id</span><span class="sxs-lookup"><span data-stu-id="70a6f-110">id</span></span>            | <span data-ttu-id="70a6f-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="70a6f-111">String</span></span>                | <span data-ttu-id="70a6f-112">Identidade do contato no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="70a6f-112">Identity of the contact within Azure Active Directory.</span></span>                                                              |
| <span data-ttu-id="70a6f-113">displayName</span><span class="sxs-lookup"><span data-stu-id="70a6f-113">displayName</span></span>   | <span data-ttu-id="70a6f-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="70a6f-114">String</span></span>                | <span data-ttu-id="70a6f-115">Nome do contato.</span><span class="sxs-lookup"><span data-stu-id="70a6f-115">Name of the contact.</span></span> <span data-ttu-id="70a6f-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70a6f-116">Required.</span></span>                                                                                      |
| <span data-ttu-id="70a6f-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="70a6f-117">emailAddress</span></span>  | <span data-ttu-id="70a6f-118">String</span><span class="sxs-lookup"><span data-stu-id="70a6f-118">String</span></span>                | <span data-ttu-id="70a6f-119">Endereço de email principal do contato.</span><span class="sxs-lookup"><span data-stu-id="70a6f-119">Primary email address of the contact.</span></span>                                                                               |
| <span data-ttu-id="70a6f-120">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="70a6f-120">mobilePhone</span></span>   | <span data-ttu-id="70a6f-121">String</span><span class="sxs-lookup"><span data-stu-id="70a6f-121">String</span></span>                | <span data-ttu-id="70a6f-122">Número do telefone celular do contato.</span><span class="sxs-lookup"><span data-stu-id="70a6f-122">Mobile phone number of the contact.</span></span>                                                                                 |
| <span data-ttu-id="70a6f-123">relação</span><span class="sxs-lookup"><span data-stu-id="70a6f-123">relationship</span></span>  | `contactRelationship` | <span data-ttu-id="70a6f-124">Relação com o usuário.</span><span class="sxs-lookup"><span data-stu-id="70a6f-124">Relationship to the user.</span></span> <span data-ttu-id="70a6f-125">Os valores possíveis são:,,,, `parent` `relative` `aide` `doctor` `guardian` `child` , `other` .</span><span class="sxs-lookup"><span data-stu-id="70a6f-125">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`.</span></span> |
| <span data-ttu-id="70a6f-126">accessConsent</span><span class="sxs-lookup"><span data-stu-id="70a6f-126">accessConsent</span></span> | <span data-ttu-id="70a6f-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="70a6f-127">Boolean</span></span>               | <span data-ttu-id="70a6f-128">Indica se o usuário foi remetido para acessar os dados dos alunos.</span><span class="sxs-lookup"><span data-stu-id="70a6f-128">Indicates whether the user has been consented to access student data.</span></span>                                               |

## <a name="json-representation"></a><span data-ttu-id="70a6f-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70a6f-129">JSON representation</span></span>

<span data-ttu-id="70a6f-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="70a6f-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relatedContact"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "contactRelationship",
  "accessConsent": true
}
```

<!-- uuid: 720F9AB6-6E7A-4A66-8B0A-37A556FF99C5
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "relatedContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


