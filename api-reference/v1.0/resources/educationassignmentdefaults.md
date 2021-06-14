---
title: Tipo de recurso educationAssignmentDefaults
description: Especifica os padrões de nível de classe respeitados por novas atribuições criadas na classe
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e990e7fe940fface9ecc33d066ce86b6cc331e4f
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912124"
---
# <a name="educationassignmentdefaults-resource-type"></a><span data-ttu-id="07704-103">Tipo de recurso educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="07704-103">educationAssignmentDefaults resource type</span></span>

<span data-ttu-id="07704-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07704-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="07704-105">Especifica os padrões de nível de classe respeitados por novas atribuições criadas na classe.</span><span class="sxs-lookup"><span data-stu-id="07704-105">Specifies class-level defaults respected by new assignments created in the class.</span></span> 

<span data-ttu-id="07704-106">Os chamadores podem continuar a especificar valores personalizados em cada criação de atribuição se não quiserem os comportamentos padrão.</span><span class="sxs-lookup"><span data-stu-id="07704-106">Callers can continue to specify custom values on each assignment creation if they Don't want the default behaviors.</span></span>

## <a name="methods"></a><span data-ttu-id="07704-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="07704-107">Methods</span></span>
|<span data-ttu-id="07704-108">Método</span><span class="sxs-lookup"><span data-stu-id="07704-108">Method</span></span>|<span data-ttu-id="07704-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="07704-109">Return type</span></span>|<span data-ttu-id="07704-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="07704-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="07704-111">Obter educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="07704-111">Get educationAssignmentDefaults</span></span>](../api/educationassignmentdefaults-get.md)|[<span data-ttu-id="07704-112">educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="07704-112">educationAssignmentDefaults</span></span>](../resources/educationassignmentdefaults.md)|<span data-ttu-id="07704-113">Leia as propriedades e as relações de um [objeto educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)</span><span class="sxs-lookup"><span data-stu-id="07704-113">Read the properties and relationships of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span>|
|[<span data-ttu-id="07704-114">Atualizar educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="07704-114">Update educationAssignmentDefaults</span></span>](../api/educationassignmentdefaults-update.md)|[<span data-ttu-id="07704-115">educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="07704-115">educationAssignmentDefaults</span></span>](../resources/educationassignmentdefaults.md)|<span data-ttu-id="07704-116">Atualize as propriedades de um [objeto educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)</span><span class="sxs-lookup"><span data-stu-id="07704-116">Update the properties of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="07704-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07704-117">Properties</span></span>
|<span data-ttu-id="07704-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07704-118">Property</span></span>|<span data-ttu-id="07704-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="07704-119">Type</span></span>|<span data-ttu-id="07704-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="07704-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07704-121">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="07704-121">addedStudentAction</span></span>|<span data-ttu-id="07704-122">educationAddedStudentAction</span><span class="sxs-lookup"><span data-stu-id="07704-122">educationAddedStudentAction</span></span>|<span data-ttu-id="07704-123">Comportamento padrão no nível de classe para lidar com alunos que são adicionados após a publicação da atribuição.</span><span class="sxs-lookup"><span data-stu-id="07704-123">Class-level default behavior for handling students who are added after the assignment is published.</span></span> <span data-ttu-id="07704-124">Os valores possíveis são: `none` e `assignIfOpen`.</span><span class="sxs-lookup"><span data-stu-id="07704-124">Possible values are: `none`, `assignIfOpen`.</span></span>|
|<span data-ttu-id="07704-125">dueTime</span><span class="sxs-lookup"><span data-stu-id="07704-125">dueTime</span></span>|<span data-ttu-id="07704-126">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="07704-126">TimeOfDay</span></span>|<span data-ttu-id="07704-127">Valor padrão de nível de classe para o campo de tempo de vencimento.</span><span class="sxs-lookup"><span data-stu-id="07704-127">Class-level default value for due time field.</span></span> <span data-ttu-id="07704-128">O valor padrão é `23:59:00`.</span><span class="sxs-lookup"><span data-stu-id="07704-128">Default value is `23:59:00`.</span></span>|
|<span data-ttu-id="07704-129">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="07704-129">notificationChannelUrl</span></span>|<span data-ttu-id="07704-130">String</span><span class="sxs-lookup"><span data-stu-id="07704-130">String</span></span>|<span data-ttu-id="07704-131">Canal Teams padrão para o qual as notificações serão enviadas.</span><span class="sxs-lookup"><span data-stu-id="07704-131">Default Teams channel to which notifications will be sent.</span></span> <span data-ttu-id="07704-132">O valor padrão é `null`.</span><span class="sxs-lookup"><span data-stu-id="07704-132">Default value is `null`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07704-133">Relações</span><span class="sxs-lookup"><span data-stu-id="07704-133">Relationships</span></span>
<span data-ttu-id="07704-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="07704-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="07704-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07704-135">JSON representation</span></span>
<span data-ttu-id="07704-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07704-136">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentDefaults",
  "openType": false
}
-->
``` json
{
  "addedStudentAction": "String",
  "dueTime": "String (timestamp)",
  "notificationChannelUrl": "String"
}
```

