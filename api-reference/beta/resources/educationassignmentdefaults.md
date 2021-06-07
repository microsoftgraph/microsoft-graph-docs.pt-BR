---
title: Tipo de recurso educationAssignmentDefaults
description: Especifica os padrões de nível de classe respeitados por novas atribuições criadas na classe
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: cdd4cb3814900f41f7cb7ee5ede407af61e9c4d7
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781062"
---
# <a name="educationassignmentdefaults-resource-type"></a><span data-ttu-id="ac9ea-103">Tipo de recurso educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="ac9ea-103">educationAssignmentDefaults resource type</span></span>

<span data-ttu-id="ac9ea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac9ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac9ea-105">Especifica os padrões de nível de classe respeitados por novas atribuições criadas na classe.</span><span class="sxs-lookup"><span data-stu-id="ac9ea-105">Specifies class-level defaults respected by new assignments created in the class.</span></span> <span data-ttu-id="ac9ea-106">Os chamadores podem continuar a especificar valores personalizados em cada criação de atribuição se não quiserem os comportamentos padrão.</span><span class="sxs-lookup"><span data-stu-id="ac9ea-106">Callers can continue to specify custom values on each assignment creation if they do not want the default behaviors.</span></span>

## <a name="methods"></a><span data-ttu-id="ac9ea-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ac9ea-107">Methods</span></span>
|<span data-ttu-id="ac9ea-108">Método</span><span class="sxs-lookup"><span data-stu-id="ac9ea-108">Method</span></span>|<span data-ttu-id="ac9ea-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ac9ea-109">Return type</span></span>|<span data-ttu-id="ac9ea-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac9ea-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ac9ea-111">Obter educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="ac9ea-111">Get educationAssignmentDefaults</span></span>](../api/educationassignmentdefaults-get.md)|[<span data-ttu-id="ac9ea-112">educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="ac9ea-112">educationAssignmentDefaults</span></span>](../resources/educationassignmentdefaults.md)|<span data-ttu-id="ac9ea-113">Leia as propriedades e as relações de um [objeto educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)</span><span class="sxs-lookup"><span data-stu-id="ac9ea-113">Read the properties and relationships of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span>|
|[<span data-ttu-id="ac9ea-114">Atualizar educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="ac9ea-114">Update educationAssignmentDefaults</span></span>](../api/educationassignmentdefaults-update.md)|[<span data-ttu-id="ac9ea-115">educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="ac9ea-115">educationAssignmentDefaults</span></span>](../resources/educationassignmentdefaults.md)|<span data-ttu-id="ac9ea-116">Atualize as propriedades de um [objeto educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)</span><span class="sxs-lookup"><span data-stu-id="ac9ea-116">Update the properties of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ac9ea-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac9ea-117">Properties</span></span>
|<span data-ttu-id="ac9ea-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac9ea-118">Property</span></span>|<span data-ttu-id="ac9ea-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac9ea-119">Type</span></span>|<span data-ttu-id="ac9ea-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac9ea-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac9ea-121">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="ac9ea-121">addedStudentAction</span></span>|<span data-ttu-id="ac9ea-122">educationAddedStudentAction</span><span class="sxs-lookup"><span data-stu-id="ac9ea-122">educationAddedStudentAction</span></span>|<span data-ttu-id="ac9ea-123">Comportamento padrão no nível de classe para lidar com alunos que são adicionados após a publicação da atribuição.</span><span class="sxs-lookup"><span data-stu-id="ac9ea-123">Class-level default behavior for handling students who are added after the assignment is published.</span></span> <span data-ttu-id="ac9ea-124">Os valores possíveis são: `none` e `assignIfOpen`.</span><span class="sxs-lookup"><span data-stu-id="ac9ea-124">Possible values are: `none`, `assignIfOpen`.</span></span>|
|<span data-ttu-id="ac9ea-125">addToCalendarAction</span><span class="sxs-lookup"><span data-stu-id="ac9ea-125">addToCalendarAction</span></span>| <span data-ttu-id="ac9ea-126">educationAddToCalendarOptions</span><span class="sxs-lookup"><span data-stu-id="ac9ea-126">educationAddToCalendarOptions</span></span>|<span data-ttu-id="ac9ea-127">Campo opcional para controlar a adição de atribuições aos calendários dos alunos e professores quando a atribuição for publicada.</span><span class="sxs-lookup"><span data-stu-id="ac9ea-127">Optional field to control the asfor adding assignments to students' and teachers' calendars when the assignment is published.</span></span> <span data-ttu-id="ac9ea-128">Os valores possíveis são: `studentsAndPublisher`, `studentsAndTeamOwners`, `none`.</span><span class="sxs-lookup"><span data-stu-id="ac9ea-128">Possible values are: `studentsAndPublisher`, `studentsAndTeamOwners`, `none`.</span></span> <span data-ttu-id="ac9ea-129">O valor padrão é `none`.</span><span class="sxs-lookup"><span data-stu-id="ac9ea-129">Default value is `none`.</span></span>|
|<span data-ttu-id="ac9ea-130">dueTime</span><span class="sxs-lookup"><span data-stu-id="ac9ea-130">dueTime</span></span>|<span data-ttu-id="ac9ea-131">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ac9ea-131">TimeOfDay</span></span>|<span data-ttu-id="ac9ea-132">Valor padrão de nível de classe para o campo de tempo de vencimento.</span><span class="sxs-lookup"><span data-stu-id="ac9ea-132">Class-level default value for due time field.</span></span> <span data-ttu-id="ac9ea-133">O valor padrão é `23:59:00`.</span><span class="sxs-lookup"><span data-stu-id="ac9ea-133">Default value is `23:59:00`.</span></span>|
|<span data-ttu-id="ac9ea-134">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="ac9ea-134">notificationChannelUrl</span></span>|<span data-ttu-id="ac9ea-135">String</span><span class="sxs-lookup"><span data-stu-id="ac9ea-135">String</span></span>|<span data-ttu-id="ac9ea-136">Canal Teams padrão para o qual as notificações serão enviadas.</span><span class="sxs-lookup"><span data-stu-id="ac9ea-136">Default Teams channel to which notifications will be sent.</span></span> <span data-ttu-id="ac9ea-137">O valor padrão é `null`.</span><span class="sxs-lookup"><span data-stu-id="ac9ea-137">Default value is `null`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac9ea-138">Relações</span><span class="sxs-lookup"><span data-stu-id="ac9ea-138">Relationships</span></span>
<span data-ttu-id="ac9ea-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ac9ea-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac9ea-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac9ea-140">JSON representation</span></span>
<span data-ttu-id="ac9ea-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac9ea-141">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentDefaults",
  "openType": false
}
-->
``` json
{
  "addedStudentAction": "none",
  "addToCalendarAction": "none",
  "dueTime": "23:59:00",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('id')/channels('id')"
}
```

