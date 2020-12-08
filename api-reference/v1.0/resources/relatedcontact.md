---
title: tipo de recurso relatedContact
description: Registro de contato relacionado a um educationUser que fornece informações para guardiões, auxílios, médicos e assim por diante.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f1dd62a2727ec2cbd6a4044b84105d739bbf9c93
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597379"
---
# <a name="relatedcontact-resource-type"></a><span data-ttu-id="d4a04-103">tipo de recurso relatedContact</span><span class="sxs-lookup"><span data-stu-id="d4a04-103">relatedContact resource type</span></span>

<span data-ttu-id="d4a04-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d4a04-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d4a04-105">Registro de contato relacionado a um [educationUser](../resources/educationuser.md) que fornece informações para guardiões, auxílios, médicos e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="d4a04-105">Contact record related to an [educationUser](../resources/educationuser.md) that provides information for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="d4a04-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d4a04-106">Properties</span></span>

| <span data-ttu-id="d4a04-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4a04-107">Property</span></span>      | <span data-ttu-id="d4a04-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4a04-108">Type</span></span>                  | <span data-ttu-id="d4a04-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4a04-109">Description</span></span>                                                                                                                               |
| :------------ | :-------------------- | :---------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d4a04-110">id</span><span class="sxs-lookup"><span data-stu-id="d4a04-110">id</span></span>            | <span data-ttu-id="d4a04-111">String</span><span class="sxs-lookup"><span data-stu-id="d4a04-111">String</span></span>                | <span data-ttu-id="d4a04-112">Identidade do contato no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d4a04-112">Identity of the contact within Azure Active Directory.</span></span>                                                                                    |
| <span data-ttu-id="d4a04-113">displayName</span><span class="sxs-lookup"><span data-stu-id="d4a04-113">displayName</span></span>   | <span data-ttu-id="d4a04-114">String</span><span class="sxs-lookup"><span data-stu-id="d4a04-114">String</span></span>                | <span data-ttu-id="d4a04-115">Nome do contato.</span><span class="sxs-lookup"><span data-stu-id="d4a04-115">Name of the contact.</span></span> <span data-ttu-id="d4a04-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4a04-116">Required.</span></span>                                                                                                            |
| <span data-ttu-id="d4a04-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d4a04-117">emailAddress</span></span>  | <span data-ttu-id="d4a04-118">String</span><span class="sxs-lookup"><span data-stu-id="d4a04-118">String</span></span>                | <span data-ttu-id="d4a04-119">Endereço de email principal do contato.</span><span class="sxs-lookup"><span data-stu-id="d4a04-119">Primary email address of the contact.</span></span>                                                                                                     |
| <span data-ttu-id="d4a04-120">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="d4a04-120">mobilePhone</span></span>   | <span data-ttu-id="d4a04-121">String</span><span class="sxs-lookup"><span data-stu-id="d4a04-121">String</span></span>                | <span data-ttu-id="d4a04-122">Número do telefone celular do contato.</span><span class="sxs-lookup"><span data-stu-id="d4a04-122">Mobile phone number of the contact.</span></span>                                                                                                       |
| <span data-ttu-id="d4a04-123">relação</span><span class="sxs-lookup"><span data-stu-id="d4a04-123">relationship</span></span>  | `contactRelationship` | <span data-ttu-id="d4a04-124">Relação com o usuário.</span><span class="sxs-lookup"><span data-stu-id="d4a04-124">Relationship to the user.</span></span> <span data-ttu-id="d4a04-125">Os valores possíveis são:,,,,, `parent` `relative` `aide` `doctor` `guardian` `child` `other` , `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="d4a04-125">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span> |
| <span data-ttu-id="d4a04-126">accessConsent</span><span class="sxs-lookup"><span data-stu-id="d4a04-126">accessConsent</span></span> | <span data-ttu-id="d4a04-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4a04-127">Boolean</span></span>               | <span data-ttu-id="d4a04-128">Indica se o usuário foi remetido para acessar os dados dos alunos.</span><span class="sxs-lookup"><span data-stu-id="d4a04-128">Indicates whether the user has been consented to access student data.</span></span>                                                                     |

## <a name="json-representation"></a><span data-ttu-id="d4a04-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4a04-129">JSON representation</span></span>

<span data-ttu-id="d4a04-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d4a04-130">The following is a JSON representation of the resource.</span></span>

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

