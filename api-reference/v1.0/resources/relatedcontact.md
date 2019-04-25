---
title: tipo de recurso relatedContact
description: Registro de contato relacionado a um educationUser que fornece informações para guardiões, auxílios, médicos e assim por diante.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7e3829de2ffeb073d8360976ce70d13985fcae39
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579405"
---
# <a name="realtedcontact-resource-type"></a><span data-ttu-id="bc896-103">tipo de recurso realtedContact</span><span class="sxs-lookup"><span data-stu-id="bc896-103">realtedContact resource type</span></span>

<span data-ttu-id="bc896-104">Registro de contato relacionado a um [educationUser](../resources/educationuser.md) que fornece informações para guardiões, auxílios, médicos e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="bc896-104">Contact record related to an [educationUser](../resources/educationuser.md) that provides information for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="bc896-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc896-105">Properties</span></span>
| <span data-ttu-id="bc896-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc896-106">Property</span></span>     | <span data-ttu-id="bc896-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc896-107">Type</span></span>   |<span data-ttu-id="bc896-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc896-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc896-109">id</span><span class="sxs-lookup"><span data-stu-id="bc896-109">id</span></span>|<span data-ttu-id="bc896-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc896-110">String</span></span>|<span data-ttu-id="bc896-111">Identidade do contato no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bc896-111">Identity of the contact within Azure Active Directory.</span></span>|
|<span data-ttu-id="bc896-112">displayName</span><span class="sxs-lookup"><span data-stu-id="bc896-112">displayName</span></span>|<span data-ttu-id="bc896-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc896-113">String</span></span>|<span data-ttu-id="bc896-114">Nome do contato.</span><span class="sxs-lookup"><span data-stu-id="bc896-114">Name of the contact.</span></span> <span data-ttu-id="bc896-115">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc896-115">Required.</span></span>|
|<span data-ttu-id="bc896-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="bc896-116">emailAddress</span></span>|<span data-ttu-id="bc896-117">String</span><span class="sxs-lookup"><span data-stu-id="bc896-117">String</span></span>|<span data-ttu-id="bc896-118">Endereço de email principal do contato.</span><span class="sxs-lookup"><span data-stu-id="bc896-118">Primary email address of the contact.</span></span>|
|<span data-ttu-id="bc896-119">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="bc896-119">mobilePhone</span></span>|<span data-ttu-id="bc896-120">String</span><span class="sxs-lookup"><span data-stu-id="bc896-120">String</span></span>|<span data-ttu-id="bc896-121">Número do telefone celular do contato.</span><span class="sxs-lookup"><span data-stu-id="bc896-121">Mobile phone number of the contact.</span></span>|
|<span data-ttu-id="bc896-122">relação</span><span class="sxs-lookup"><span data-stu-id="bc896-122">relationship</span></span>|`contactRelationship`|<span data-ttu-id="bc896-123">Relação com o usuário.</span><span class="sxs-lookup"><span data-stu-id="bc896-123">Relationship to the user.</span></span> <span data-ttu-id="bc896-124">Os valores possíveis `parent`são `relative`: `aide` `doctor` `guardian` `child`,,,, `other`, `unknownFutureValue`,.</span><span class="sxs-lookup"><span data-stu-id="bc896-124">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="bc896-125">accessConsent</span><span class="sxs-lookup"><span data-stu-id="bc896-125">accessConsent</span></span>|<span data-ttu-id="bc896-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc896-126">Boolean</span></span>|<span data-ttu-id="bc896-127">Indica se o usuário foi remetido para acessar os dados dos alunos.</span><span class="sxs-lookup"><span data-stu-id="bc896-127">Indicates whether the user has been consented to access student data.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc896-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc896-128">JSON representation</span></span>

<span data-ttu-id="bc896-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc896-129">The following is a JSON representation of the resource.</span></span>

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
