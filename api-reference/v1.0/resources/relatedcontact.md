---
title: tipo de recurso relatedContact
description: Registro de contato relacionado a um educationUser que fornece informações para guardiões, auxílios, médicos e assim por diante.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: adea95729dd4e6558885223245a7225811f14677
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002944"
---
# <a name="realtedcontact-resource-type"></a><span data-ttu-id="a9da2-103">tipo de recurso realtedContact</span><span class="sxs-lookup"><span data-stu-id="a9da2-103">realtedContact resource type</span></span>

<span data-ttu-id="a9da2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9da2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a9da2-105">Registro de contato relacionado a um [educationUser](../resources/educationuser.md) que fornece informações para guardiões, auxílios, médicos e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="a9da2-105">Contact record related to an [educationUser](../resources/educationuser.md) that provides information for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="a9da2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9da2-106">Properties</span></span>

| <span data-ttu-id="a9da2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9da2-107">Property</span></span>      | <span data-ttu-id="a9da2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9da2-108">Type</span></span>                  | <span data-ttu-id="a9da2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9da2-109">Description</span></span>                                                                                                                               |
| :------------ | :-------------------- | :---------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="a9da2-110">id</span><span class="sxs-lookup"><span data-stu-id="a9da2-110">id</span></span>            | <span data-ttu-id="a9da2-111">String</span><span class="sxs-lookup"><span data-stu-id="a9da2-111">String</span></span>                | <span data-ttu-id="a9da2-112">Identidade do contato no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a9da2-112">Identity of the contact within Azure Active Directory.</span></span>                                                                                    |
| <span data-ttu-id="a9da2-113">displayName</span><span class="sxs-lookup"><span data-stu-id="a9da2-113">displayName</span></span>   | <span data-ttu-id="a9da2-114">String</span><span class="sxs-lookup"><span data-stu-id="a9da2-114">String</span></span>                | <span data-ttu-id="a9da2-115">Nome do contato.</span><span class="sxs-lookup"><span data-stu-id="a9da2-115">Name of the contact.</span></span> <span data-ttu-id="a9da2-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9da2-116">Required.</span></span>                                                                                                            |
| <span data-ttu-id="a9da2-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a9da2-117">emailAddress</span></span>  | <span data-ttu-id="a9da2-118">String</span><span class="sxs-lookup"><span data-stu-id="a9da2-118">String</span></span>                | <span data-ttu-id="a9da2-119">Endereço de email principal do contato.</span><span class="sxs-lookup"><span data-stu-id="a9da2-119">Primary email address of the contact.</span></span>                                                                                                     |
| <span data-ttu-id="a9da2-120">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="a9da2-120">mobilePhone</span></span>   | <span data-ttu-id="a9da2-121">String</span><span class="sxs-lookup"><span data-stu-id="a9da2-121">String</span></span>                | <span data-ttu-id="a9da2-122">Número do telefone celular do contato.</span><span class="sxs-lookup"><span data-stu-id="a9da2-122">Mobile phone number of the contact.</span></span>                                                                                                       |
| <span data-ttu-id="a9da2-123">relação</span><span class="sxs-lookup"><span data-stu-id="a9da2-123">relationship</span></span>  | `contactRelationship` | <span data-ttu-id="a9da2-124">Relação com o usuário.</span><span class="sxs-lookup"><span data-stu-id="a9da2-124">Relationship to the user.</span></span> <span data-ttu-id="a9da2-125">Os valores possíveis são:,,,,, `parent` `relative` `aide` `doctor` `guardian` `child` `other` , `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="a9da2-125">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span> |
| <span data-ttu-id="a9da2-126">accessConsent</span><span class="sxs-lookup"><span data-stu-id="a9da2-126">accessConsent</span></span> | <span data-ttu-id="a9da2-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9da2-127">Boolean</span></span>               | <span data-ttu-id="a9da2-128">Indica se o usuário foi remetido para acessar os dados dos alunos.</span><span class="sxs-lookup"><span data-stu-id="a9da2-128">Indicates whether the user has been consented to access student data.</span></span>                                                                     |

## <a name="json-representation"></a><span data-ttu-id="a9da2-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9da2-129">JSON representation</span></span>

<span data-ttu-id="a9da2-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a9da2-130">The following is a JSON representation of the resource.</span></span>

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

