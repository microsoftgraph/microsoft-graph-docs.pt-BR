---
title: tipo de recurso de relatedContact
description: Registro de contato relacionado a um educationUser que fornece informações para responsáveis, auxílios, os médicos e assim por diante.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7e3829de2ffeb073d8360976ce70d13985fcae39
ms.sourcegitcommit: d6209114cbbe8072e3ecf7eba23819ae5ace7db5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2019
ms.locfileid: "29694486"
---
# <a name="realtedcontact-resource-type"></a><span data-ttu-id="2ddf6-103">tipo de recurso de realtedContact</span><span class="sxs-lookup"><span data-stu-id="2ddf6-103">realtedContact resource type</span></span>

<span data-ttu-id="2ddf6-104">Entre em contato com o registro de um [educationUser](../resources/educationuser.md) que fornece informações para responsáveis, auxílios, os médicos e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="2ddf6-104">Contact record related to an [educationUser](../resources/educationuser.md) that provides information for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="2ddf6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ddf6-105">Properties</span></span>
| <span data-ttu-id="2ddf6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ddf6-106">Property</span></span>     | <span data-ttu-id="2ddf6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ddf6-107">Type</span></span>   |<span data-ttu-id="2ddf6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ddf6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ddf6-109">id</span><span class="sxs-lookup"><span data-stu-id="2ddf6-109">id</span></span>|<span data-ttu-id="2ddf6-110">String</span><span class="sxs-lookup"><span data-stu-id="2ddf6-110">String</span></span>|<span data-ttu-id="2ddf6-111">Identidade do contato dentro do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2ddf6-111">Identity of the contact within Azure Active Directory.</span></span>|
|<span data-ttu-id="2ddf6-112">displayName</span><span class="sxs-lookup"><span data-stu-id="2ddf6-112">displayName</span></span>|<span data-ttu-id="2ddf6-113">String</span><span class="sxs-lookup"><span data-stu-id="2ddf6-113">String</span></span>|<span data-ttu-id="2ddf6-114">Nome do contato.</span><span class="sxs-lookup"><span data-stu-id="2ddf6-114">Name of the contact.</span></span> <span data-ttu-id="2ddf6-115">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ddf6-115">Required.</span></span>|
|<span data-ttu-id="2ddf6-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="2ddf6-116">emailAddress</span></span>|<span data-ttu-id="2ddf6-117">String</span><span class="sxs-lookup"><span data-stu-id="2ddf6-117">String</span></span>|<span data-ttu-id="2ddf6-118">Endereço de email principal do contato.</span><span class="sxs-lookup"><span data-stu-id="2ddf6-118">Primary email address of the contact.</span></span>|
|<span data-ttu-id="2ddf6-119">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="2ddf6-119">mobilePhone</span></span>|<span data-ttu-id="2ddf6-120">String</span><span class="sxs-lookup"><span data-stu-id="2ddf6-120">String</span></span>|<span data-ttu-id="2ddf6-121">Número de telefone celular do contato.</span><span class="sxs-lookup"><span data-stu-id="2ddf6-121">Mobile phone number of the contact.</span></span>|
|<span data-ttu-id="2ddf6-122">Relação</span><span class="sxs-lookup"><span data-stu-id="2ddf6-122">relationship</span></span>|`contactRelationship`|<span data-ttu-id="2ddf6-123">Relacionamento ao usuário.</span><span class="sxs-lookup"><span data-stu-id="2ddf6-123">Relationship to the user.</span></span> <span data-ttu-id="2ddf6-124">Os valores possíveis são `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="2ddf6-124">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="2ddf6-125">accessConsent</span><span class="sxs-lookup"><span data-stu-id="2ddf6-125">accessConsent</span></span>|<span data-ttu-id="2ddf6-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ddf6-126">Boolean</span></span>|<span data-ttu-id="2ddf6-127">Indica se o usuário foi aceitou para acessar dados de student.</span><span class="sxs-lookup"><span data-stu-id="2ddf6-127">Indicates whether the user has been consented to access student data.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ddf6-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ddf6-128">JSON representation</span></span>

<span data-ttu-id="2ddf6-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ddf6-129">The following is a JSON representation of the resource.</span></span>

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
