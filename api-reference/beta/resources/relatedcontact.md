---
title: tipo de recurso relatedContact
description: Registro de contato relacionado a um educationUser que fornece informações para guardiões, auxílios, médicos e assim por diante.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7eb8f39c30343412584e63fa1e8c3382db4fa9c6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521184"
---
# <a name="relatedcontact-resource-type"></a><span data-ttu-id="cb003-103">tipo de recurso relatedContact</span><span class="sxs-lookup"><span data-stu-id="cb003-103">relatedContact resource type</span></span>

<span data-ttu-id="cb003-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cb003-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb003-105">Registro de contato relacionado a um [educationUser](../resources/educationuser.md) que fornece informações para guardiões, auxílios, médicos e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="cb003-105">Contact record related to an [educationUser](../resources/educationuser.md) that provides information for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="cb003-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb003-106">Properties</span></span>

| <span data-ttu-id="cb003-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb003-107">Property</span></span>      | <span data-ttu-id="cb003-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb003-108">Type</span></span>                  | <span data-ttu-id="cb003-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb003-109">Description</span></span>                                                                                                         |
| :------------ | :-------------------- | :------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="cb003-110">id</span><span class="sxs-lookup"><span data-stu-id="cb003-110">id</span></span>            | <span data-ttu-id="cb003-111">String</span><span class="sxs-lookup"><span data-stu-id="cb003-111">String</span></span>                | <span data-ttu-id="cb003-112">Identidade do contato no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cb003-112">Identity of the contact within Azure Active Directory.</span></span>                                                              |
| <span data-ttu-id="cb003-113">displayName</span><span class="sxs-lookup"><span data-stu-id="cb003-113">displayName</span></span>   | <span data-ttu-id="cb003-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb003-114">String</span></span>                | <span data-ttu-id="cb003-115">Nome do contato.</span><span class="sxs-lookup"><span data-stu-id="cb003-115">Name of the contact.</span></span> <span data-ttu-id="cb003-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb003-116">Required.</span></span>                                                                                      |
| <span data-ttu-id="cb003-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="cb003-117">emailAddress</span></span>  | <span data-ttu-id="cb003-118">String</span><span class="sxs-lookup"><span data-stu-id="cb003-118">String</span></span>                | <span data-ttu-id="cb003-119">Endereço de email principal do contato.</span><span class="sxs-lookup"><span data-stu-id="cb003-119">Primary email address of the contact.</span></span>                                                                               |
| <span data-ttu-id="cb003-120">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="cb003-120">mobilePhone</span></span>   | <span data-ttu-id="cb003-121">String</span><span class="sxs-lookup"><span data-stu-id="cb003-121">String</span></span>                | <span data-ttu-id="cb003-122">Número do telefone celular do contato.</span><span class="sxs-lookup"><span data-stu-id="cb003-122">Mobile phone number of the contact.</span></span>                                                                                 |
| <span data-ttu-id="cb003-123">relação</span><span class="sxs-lookup"><span data-stu-id="cb003-123">relationship</span></span>  | `contactRelationship` | <span data-ttu-id="cb003-124">Relação com o usuário.</span><span class="sxs-lookup"><span data-stu-id="cb003-124">Relationship to the user.</span></span> <span data-ttu-id="cb003-125">Os valores possíveis `parent`são `relative`: `aide` `doctor` `guardian`,,, `child`, `other`,.</span><span class="sxs-lookup"><span data-stu-id="cb003-125">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`.</span></span> |
| <span data-ttu-id="cb003-126">accessConsent</span><span class="sxs-lookup"><span data-stu-id="cb003-126">accessConsent</span></span> | <span data-ttu-id="cb003-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb003-127">Boolean</span></span>               | <span data-ttu-id="cb003-128">Indica se o usuário foi remetido para acessar os dados dos alunos.</span><span class="sxs-lookup"><span data-stu-id="cb003-128">Indicates whether the user has been consented to access student data.</span></span>                                               |

## <a name="json-representation"></a><span data-ttu-id="cb003-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb003-129">JSON representation</span></span>

<span data-ttu-id="cb003-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb003-130">The following is a JSON representation of the resource.</span></span>

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
