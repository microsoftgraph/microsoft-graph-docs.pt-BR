---
title: tipo de recurso de relatedContact
description: Registro de contato relacionado a um educationUser que fornece informações para responsáveis, auxílios, os médicos e assim por diante.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d29cf93154e2c032ac7010372e3f116f2a1dd46c
ms.sourcegitcommit: d6209114cbbe8072e3ecf7eba23819ae5ace7db5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2019
ms.locfileid: "29694472"
---
# <a name="relatedcontact-resource-type"></a><span data-ttu-id="9d287-103">tipo de recurso de relatedContact</span><span class="sxs-lookup"><span data-stu-id="9d287-103">relatedContact resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d287-104">Entre em contato com o registro de um [educationUser](../resources/educationuser.md) que fornece informações para responsáveis, auxílios, os médicos e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="9d287-104">Contact record related to an [educationUser](../resources/educationuser.md) that provides inforation for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="9d287-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d287-105">Properties</span></span>
| <span data-ttu-id="9d287-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d287-106">Property</span></span>     | <span data-ttu-id="9d287-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d287-107">Type</span></span>   |<span data-ttu-id="9d287-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d287-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d287-109">id</span><span class="sxs-lookup"><span data-stu-id="9d287-109">id</span></span>|<span data-ttu-id="9d287-110">String</span><span class="sxs-lookup"><span data-stu-id="9d287-110">String</span></span>|<span data-ttu-id="9d287-111">Identidade do contato dentro do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9d287-111">Identity of the contact within Azure Active Directory.</span></span>|
|<span data-ttu-id="9d287-112">displayName</span><span class="sxs-lookup"><span data-stu-id="9d287-112">displayName</span></span>|<span data-ttu-id="9d287-113">String</span><span class="sxs-lookup"><span data-stu-id="9d287-113">String</span></span>|<span data-ttu-id="9d287-114">Nome do contato.</span><span class="sxs-lookup"><span data-stu-id="9d287-114">Name of the contact.</span></span> <span data-ttu-id="9d287-115">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d287-115">Required.</span></span>|
|<span data-ttu-id="9d287-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9d287-116">emailAddress</span></span>|<span data-ttu-id="9d287-117">String</span><span class="sxs-lookup"><span data-stu-id="9d287-117">String</span></span>|<span data-ttu-id="9d287-118">Endereço de email principal do contato.</span><span class="sxs-lookup"><span data-stu-id="9d287-118">Primary email address of the contact.</span></span>|
|<span data-ttu-id="9d287-119">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="9d287-119">mobilePhone</span></span>|<span data-ttu-id="9d287-120">String</span><span class="sxs-lookup"><span data-stu-id="9d287-120">String</span></span>|<span data-ttu-id="9d287-121">Número de telefone celular do contato.</span><span class="sxs-lookup"><span data-stu-id="9d287-121">Mobile phone number of the contact.</span></span>|
|<span data-ttu-id="9d287-122">Relação</span><span class="sxs-lookup"><span data-stu-id="9d287-122">relationship</span></span>|`contactRelationship`|<span data-ttu-id="9d287-123">Relacionamento ao usuário.</span><span class="sxs-lookup"><span data-stu-id="9d287-123">Relationship to the user.</span></span> <span data-ttu-id="9d287-124">Os valores possíveis são `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="9d287-124">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="9d287-125">accessConsent</span><span class="sxs-lookup"><span data-stu-id="9d287-125">accessConsent</span></span>|<span data-ttu-id="9d287-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d287-126">Boolean</span></span>|<span data-ttu-id="9d287-127">Indica se o usuário foi aceitou para acessar dados de student.</span><span class="sxs-lookup"><span data-stu-id="9d287-127">Indicates whether the user has been consented to access student data.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d287-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d287-128">JSON representation</span></span>

<span data-ttu-id="9d287-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d287-129">The following is a JSON representation of the resource.</span></span>

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
