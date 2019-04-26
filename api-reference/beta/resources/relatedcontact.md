---
title: tipo de recurso relatedContact
description: Registro de contato relacionado a um educationUser que fornece informações para guardiões, auxílios, médicos e assim por diante.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d29cf93154e2c032ac7010372e3f116f2a1dd46c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343879"
---
# <a name="relatedcontact-resource-type"></a><span data-ttu-id="bedbd-103">tipo de recurso relatedContact</span><span class="sxs-lookup"><span data-stu-id="bedbd-103">relatedContact resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bedbd-104">Registro de contato relacionado a um [educationUser](../resources/educationuser.md) que fornece inforation para guardiões, auxílios, médicos e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="bedbd-104">Contact record related to an [educationUser](../resources/educationuser.md) that provides inforation for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="bedbd-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bedbd-105">Properties</span></span>
| <span data-ttu-id="bedbd-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bedbd-106">Property</span></span>     | <span data-ttu-id="bedbd-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="bedbd-107">Type</span></span>   |<span data-ttu-id="bedbd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bedbd-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bedbd-109">id</span><span class="sxs-lookup"><span data-stu-id="bedbd-109">id</span></span>|<span data-ttu-id="bedbd-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bedbd-110">String</span></span>|<span data-ttu-id="bedbd-111">Identidade do contato no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bedbd-111">Identity of the contact within Azure Active Directory.</span></span>|
|<span data-ttu-id="bedbd-112">displayName</span><span class="sxs-lookup"><span data-stu-id="bedbd-112">displayName</span></span>|<span data-ttu-id="bedbd-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bedbd-113">String</span></span>|<span data-ttu-id="bedbd-114">Nome do contato.</span><span class="sxs-lookup"><span data-stu-id="bedbd-114">Name of the contact.</span></span> <span data-ttu-id="bedbd-115">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bedbd-115">Required.</span></span>|
|<span data-ttu-id="bedbd-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="bedbd-116">emailAddress</span></span>|<span data-ttu-id="bedbd-117">String</span><span class="sxs-lookup"><span data-stu-id="bedbd-117">String</span></span>|<span data-ttu-id="bedbd-118">Endereço de email principal do contato.</span><span class="sxs-lookup"><span data-stu-id="bedbd-118">Primary email address of the contact.</span></span>|
|<span data-ttu-id="bedbd-119">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="bedbd-119">mobilePhone</span></span>|<span data-ttu-id="bedbd-120">String</span><span class="sxs-lookup"><span data-stu-id="bedbd-120">String</span></span>|<span data-ttu-id="bedbd-121">Número do telefone celular do contato.</span><span class="sxs-lookup"><span data-stu-id="bedbd-121">Mobile phone number of the contact.</span></span>|
|<span data-ttu-id="bedbd-122">relação</span><span class="sxs-lookup"><span data-stu-id="bedbd-122">relationship</span></span>|`contactRelationship`|<span data-ttu-id="bedbd-123">Relação com o usuário.</span><span class="sxs-lookup"><span data-stu-id="bedbd-123">Relationship to the user.</span></span> <span data-ttu-id="bedbd-124">Os valores possíveis `parent`são `relative`: `aide` `doctor` `guardian` `child`,,,, `other`, `unknownFutureValue`,.</span><span class="sxs-lookup"><span data-stu-id="bedbd-124">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="bedbd-125">accessConsent</span><span class="sxs-lookup"><span data-stu-id="bedbd-125">accessConsent</span></span>|<span data-ttu-id="bedbd-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="bedbd-126">Boolean</span></span>|<span data-ttu-id="bedbd-127">Indica se o usuário foi remetido para acessar os dados dos alunos.</span><span class="sxs-lookup"><span data-stu-id="bedbd-127">Indicates whether the user has been consented to access student data.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bedbd-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bedbd-128">JSON representation</span></span>

<span data-ttu-id="bedbd-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bedbd-129">The following is a JSON representation of the resource.</span></span>

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
