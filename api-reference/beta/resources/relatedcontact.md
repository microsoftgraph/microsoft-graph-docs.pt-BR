---
title: tipo de recurso relatedContact
description: Registro de contato relacionado a um educationUser que fornece informações para tutores, auxiliares, médicos e assim por diante.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4859492f016b88a39c375d3556270f5496b8b318
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035950"
---
# <a name="relatedcontact-resource-type"></a><span data-ttu-id="39ce5-103">tipo de recurso relatedContact</span><span class="sxs-lookup"><span data-stu-id="39ce5-103">relatedContact resource type</span></span>

<span data-ttu-id="39ce5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39ce5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39ce5-105">Registro de contato relacionado a [um educationUser](../resources/educationuser.md) que fornece informações para tutores, auxiliares, médicos e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="39ce5-105">Contact record related to an [educationUser](../resources/educationuser.md) that provides information for guardians, aides, doctors, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="39ce5-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="39ce5-106">Methods</span></span>

| <span data-ttu-id="39ce5-107">Método</span><span class="sxs-lookup"><span data-stu-id="39ce5-107">Method</span></span>                                    | <span data-ttu-id="39ce5-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="39ce5-108">Return Type</span></span>                   | <span data-ttu-id="39ce5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="39ce5-109">Description</span></span>                                                             |
| :---------------------------------------- | :---------------------------- | :---------------------------------------------------------------------- |
| [<span data-ttu-id="39ce5-110">Update</span><span class="sxs-lookup"><span data-stu-id="39ce5-110">Update</span></span>](../api/relatedcontact-update.md) | <span data-ttu-id="39ce5-111">**coleção relatedContact**</span><span class="sxs-lookup"><span data-stu-id="39ce5-111">**relatedContact** collection</span></span> | <span data-ttu-id="39ce5-112">Atualizar os **relatedContacts** para um [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="39ce5-112">Update the **relatedContacts** for an [educationUser](educationuser.md)</span></span> |

## <a name="properties"></a><span data-ttu-id="39ce5-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="39ce5-113">Properties</span></span>

| <span data-ttu-id="39ce5-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39ce5-114">Property</span></span>      | <span data-ttu-id="39ce5-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="39ce5-115">Type</span></span>                | <span data-ttu-id="39ce5-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="39ce5-116">Description</span></span>                                                                                                                                |
| :------------ | :------------------ | :----------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="39ce5-117">displayName</span><span class="sxs-lookup"><span data-stu-id="39ce5-117">displayName</span></span>   | <span data-ttu-id="39ce5-118">String</span><span class="sxs-lookup"><span data-stu-id="39ce5-118">String</span></span>              | <span data-ttu-id="39ce5-119">Nome do contato.</span><span class="sxs-lookup"><span data-stu-id="39ce5-119">Name of the contact.</span></span> <span data-ttu-id="39ce5-120">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39ce5-120">Required.</span></span>                                                                                                             |
| <span data-ttu-id="39ce5-121">accessConsent</span><span class="sxs-lookup"><span data-stu-id="39ce5-121">accessConsent</span></span> | <span data-ttu-id="39ce5-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="39ce5-122">Boolean</span></span>             | <span data-ttu-id="39ce5-123">Indica se o usuário foi consentido para acessar dados de alunos.</span><span class="sxs-lookup"><span data-stu-id="39ce5-123">Indicates whether the user has been consented to access student data.</span></span>                                                                      |
| <span data-ttu-id="39ce5-124">emailAddress</span><span class="sxs-lookup"><span data-stu-id="39ce5-124">emailAddress</span></span>  | <span data-ttu-id="39ce5-125">String</span><span class="sxs-lookup"><span data-stu-id="39ce5-125">String</span></span>              | <span data-ttu-id="39ce5-126">Endereço de email do contato.</span><span class="sxs-lookup"><span data-stu-id="39ce5-126">Email address of the contact.</span></span>                                                                                                              |
| <span data-ttu-id="39ce5-127">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="39ce5-127">mobilePhone</span></span>   | <span data-ttu-id="39ce5-128">String</span><span class="sxs-lookup"><span data-stu-id="39ce5-128">String</span></span>              | <span data-ttu-id="39ce5-129">Número de telefone celular do contato.</span><span class="sxs-lookup"><span data-stu-id="39ce5-129">Mobile phone number of the contact.</span></span>                                                                                                        |
| <span data-ttu-id="39ce5-130">relação</span><span class="sxs-lookup"><span data-stu-id="39ce5-130">relationship</span></span>  | <span data-ttu-id="39ce5-131">contactRelationship</span><span class="sxs-lookup"><span data-stu-id="39ce5-131">contactRelationship</span></span> | <span data-ttu-id="39ce5-132">Relação com o usuário.</span><span class="sxs-lookup"><span data-stu-id="39ce5-132">Relationship to the user.</span></span> <span data-ttu-id="39ce5-133">Os valores possíveis são: `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="39ce5-133">Possible values are: `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="39ce5-134">Relações</span><span class="sxs-lookup"><span data-stu-id="39ce5-134">Relationships</span></span>

<span data-ttu-id="39ce5-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="39ce5-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="39ce5-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="39ce5-136">JSON representation</span></span>

<span data-ttu-id="39ce5-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="39ce5-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.relatedContact"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.relatedContact",
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "String",
  "accessConsent": "Boolean"
}
```
